Instructions for Maintaining The Timeline

#Open/View the Timeline in Google Chrome
1. Open an Incoginto Chrome Browser. This will block your Browser from cacheing your files and allow you to view changes as you make them.
2. Copy and Paste the "Timeline" directory path into the address bar of Google Chrome
3. Click on Timline.html

NOTE: The timeline will function appropriately in Google Chrome, Firefox, and Safari. There is a slight animation rendering problem with Microsoft Edge. It will not work with Internet Explorer.

#Setup editing environment
1. Open a text editor like "Atom"
2. File>Add Project Folder
3. Navigate to the Timeline directory

#Adding a point to the Timeline
1. Open Timeline.html
2. Navigate to the <!-- Content --> section
3. Copy an existing point to your clipboard
    3a. This is everything from <!--Point #: Point Name Date --> to </div> and include (1) h1, (1) h2, and (1) p
4. Rename the comment tag <!-- Point #: Point Name Date --> to be relevant to the new content
5. Change the # in the "id" tag in "<div class="point" id="point-#"></div>" to match the new point number noted in Step 4.
6. Change the # in the "id" tag in "<div class="vertical-line" id="vertical-line-#"></div>" to match the new point number noted in Step 4 and 5.
7. Change the # in the "id" tag in "<div class="content" id="content-#">" to match the new point number noted in Step 4,5 and 6.
8. Update the h1, h2, and p tags to include the appropriate title, date and description respectively.
9. Open the Styles.css file
10. Navigate to the "Timeline Item Positioning" section in the Document
11. Copy the last row of "--item-#-position: %vw;" to your clipboard
12. Paste from your clipboard to the next line
13. Change the # in "--item-$-position: %vw" to match the # from Step 4.
14. Change the % in "--item-$-position: %vw" to match the expected position for the new item on the timeline. This can always be adjusted later
15. Navigate to the "Timeline Date Content" section in the document
16. Copy everything from one of the previous "Content Items" to your clipboard
17. Paste from your clipboard to the next line below the last "Content Item"
18. Rename "Content Item #" to match the # from Step 5.
19. Change all "#idtags-#" to match the # from Step 5.
    13a. Example: #content-2 --> #content-3
20. Change all #'s in "var(--item-#-position)" to match the # from Step 4 and 13.
21. Under the "#point-#" tag, change the {url} in "background-image: url("Resources/{url}.jpeg")" to point to the desired icon.
    16a. All icons for the timeline should be saved in the Resources folder
    16b. All icons should be 255px x 255px in size
22. Save file and view updates in Chrome. If position of item need to be adjusted, adjust the "%vw" from Step 14 as needed.

NOTE: %vw positions for items will need to be coordinated and cross-referenced with %vw from the date labels. Manage all the positions in the "Timeline Item Positioning" section at the top of the Styles.css document


#Adding a date label to the Timeline
1. Open Timeline.html
2. Identify the "Year Labels" section in the document. This is where labels will be added
3. Copy one of the previous labels in the section to your clipboard
4. Paste from your clipboard to the appropriate chronological place in the label list
5. Change the "id" to equal "label-[date of label inserted here]"
6. Change the date to match the date of desired label
7. Open Styles.css
8. Navigate to the "Timeline Item Positioning" section in the Document
9. Copy the last row of "--position-[date]: %vw;" to your clipboard
10. Paste from your clipboard to the next line or create a new date section header and paste there
11. Change the [date] in "--position-[date]: %vw;" to match the date label from Step 5.
12. Change the % in "--position-[date]: %vw;" to match the expected position for the new date label on the timeline. This can always be adjusted later
8. Navigate to the Date labels section in the document
9. Copy one of the previous date label styles to your clipboard
10. Paste from your clipboard to the appropriate chronological place in the label styles list
11. Change "#label-[date]" to match the id from Step 5
12. Change the [date] in "left: var(--position-[date]);" to match the date from Step 5.
13. If a different color is desired, replace the color tag with the desired hex code

NOTE: If date labels move, content/point positions will also need to be adjusted. Manage all the positions in the "Timeline Item Positioning" section at the top of the Styles.css document
