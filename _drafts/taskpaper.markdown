---
layout: post
title: Taskpaper
date: '2016-04-08 02:37:00'
---

Taskpaper
===
Thursday, April 7, 2016

Version 3 of TaskPaper has just launched. I find it to be a great tool for keeping a todo list, as well as planning what to do. 

I tweeted this when I first starting using version 3:

> QUOTE

I've tried a lot of the apps for lists and prioritization. All of them fall short of what works for me. My system is a cobbled together hybrid of GTD, Eisenhower and Nine Rocks. I'm not suggesting you adopt my system, you should find your own. I am suggesting that Taskpaper might be the thing that best *adapts* to anyones system. 

There are three main reasons I love this tool.

##Reason one
*It's just text*

As far as User Experience, Taskpaper can't be beat (for me). Real talk time: *It's just text.* There is nothing fancy. It looks like a text editor.

![Taskpaper 3](https://www.taskpaper.com/assets/img/desktop.jpg)

It behaves like a text editor. Simple text tools like writing, cut, copy, and paste, with some drag and drop. No feature bloat, and the text experience I am used to and enjoy.

I use text for the primary artifact of my work, both the day job as a Technical Project Manager, and the side jobs as a cofounder of [Rigging Dojo](http://www.riggingdojo.com) and another _secret thing_ to be revealed later. So this is a nice boon for me. It has a limited UI, it's not shiny, or confusing to use. 

It's so refreshing to just type words. 


##Reason two
*It organizes wonderfully.*
 
 Task paper let's you organize how you need to. I'll go over the way I am currently using it, and how I might begin to use it in a minute. 
 
**First, the basics.**
 
The basic rules for organization are text based. Need a project? Type a word or phrase with a colon at the end.

	This is a project:

Hit return, tab in, and start typing a task or note for the project. You don't need to do anything special for the note, just type. For an actionable task simply start that line with a dash.

	This is a note
	- This is a task
	
There's a simple tagging mechanism built in that will allow you to filter, and search your tasks. Simply type:

	- some task @someTag
	
**Searching**
There's a little search box in the top right of the UI that you can use to search for things. It's very smart, so you can type 'not @someTag' to omit everything with that particular tag. 

But the real power of the Taskpaper search is in the Saved Searches. Some where in your document, make a new task, and follow the saved search syntax. The search will appear in your sidebar for quick access and filtering. 

	@search(@someTag and not @done)
Shows you everything with the tag, that is not done. 

	@search(@due and not @done)
If you use the @due tag, and it's date modifiers this can be really helpful to figure out what to do by what time.



##Reason three
*The system is Open and deep, if you want it to be* 
 
 You can extend Taskpapaer with a bunch of hacks and stuff to make it bend to your workflow, versus the other way around. 
 
You have to get your development hands a little dirty. But trying these things out is pretty safe, and can teach you a lot about your mac, Taskpaper itself, and software development at a high level.
 
**Themes**
There isn't a theme chooser (yet), but you can customize everything you see. You might need to learn or brush up on some light web dev, but it's not that difficult to get rolling. You can find info and how-to's on Taskpaper [support](http://support.hogbaysoftware.com/t/taskpaper-extensions-wiki/1628). 

**Capture**
Since "it's just text," you'll be typing or pasting things from other sources, like your email client, the web, etc. This is a great opportunity for automation. Many people are discussing capturing text to Taskpaper. Here's the trick I use. 

I set up an Automator service to 'Run JavaScript'. So now I can simply select text _anywhere_ on my Mac, and hit a hotkey to Capture the selected text to my Taskpaper Inbox. Capture the text from anywhere, add it to the inbox to think about it later. From anywhere you guys! 

I found this script [here](http://support.hogbaysoftware.com/t/basic-script-to-add-selected-text-to-taskpaper-3-inbox/1681/5), and modified it just a little. See that link for the directions. Here's the full code:

	function run(input, parameters) {
	var selectedText = input[0]
	var TaskPaper = Application('TaskPaper')
	// Send it to TaskPaper Inbox
	TaskPaper.documents[0].evaluate({
		script: TPContext.toString(),
		withOptions: {text: selectedText }
	});
	function TPContext(editor, options) {
		var outline = editor.outline;
		var inbox = outline.evaluateItemPath("//Inbox:")[0];
		var items = ItemSerializer.deserializeItems(options.text, outline, ItemSerializer.TEXTMimeType);
		if (!inbox) {
			inbox = outline.createItem("Inbox:");
			outline.root.insertChildrenBefore(inbox, outline.root.firstChild);
		}
		inbox.insertChildrenBefore(items, inbox.firstChild);
	}
		return input;
	}

**Other scripts**
 There's so many awesome things you can script. Here's how to [install and run a script](http://support.foldingtext.com/t/how-do-i-run-install-a-script/1740?u=jessegrosjean). And this is a great reference for [Themes and Scripts](http://support.hogbaysoftware.com/t/taskpaper-extensions-wiki/1628).
 
##My workflow  

 Here's a demo of how I'm using Taskpaper.
 
 
##What's next?
I'd like to hook up to Siri and Reminders to flush out all the ways I'd like to input to Taskpaper. More on that as I figure it out.
 
 Questions? Feedback? Find me [@chad_g_moore](http://www.twitter.com/@chad_g_moore).