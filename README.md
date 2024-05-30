## Simple script to convert an Uptime.app summary to a page of formatted text.

I like Uptime, but I find the format tedious – I'd much rather just read some text than have to click through a bunch of cards.

After digging around in the source I found the content is delivered to the front-end as JSON. This script takes the JSON and creates a readable document from it.

1. Open index.html locally in your browser.
2. Log into your Uptime account and find the hack you want to read. Open the web inspector and reload the page.
3. In Safari, under the Sources tab, there should be a folder called XHRs. In there, there'll be a file with the same name as the content ID in the address bar. If the folder isn't there, reload the page and it should appear. Click the file and copy the contents.
4. In Chrome, go to the Application tab, find the 'Frames and XHR folder', look through the files until you find the one that contains the title in the first line (beginning {id:). Right click and select 'Copy value'.
5. Paste the JSON into the textarea and click 'Extract fields'. All being well, you should see the content printed below.
