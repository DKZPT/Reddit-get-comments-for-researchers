<img src="https://camo.githubusercontent.com/ce8bc12cf25c8c9ca787cf95e3693d5a17f5f4bb2b8dd5c272b88404f7ebf476/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4d616465253230776974682d507974686f6e332d627269676874677265656e" alt="Python">

<h1>About the project</h1>

This project enables the extraction comments from Reddit plataform using the API provided by them, and saves them into a csv file. 

To use this tool, you need to create an API https://www.reddit.com/prefs/apps/

The tool supports three modes of operation based on the command-line arguments provided:
Use the <b>--source</b> argument followed by the path to a JSON file containing a list of Reddit post IDs. Example command:
python reddit.py --source path/to/file.json

To extract comments using specific <b>post IDs</b>, use the -i argument followed by the IDs, separated by commas. Example command:
python reddit.py -i "id1,id2,id3"

To extract comments from specific posts via <b>URLs</b>, use the -u argument followed by the full URLs, separated by commas. Example command:
python reddit.py -u "url1,url2,url3"

<h1>Installer</h1>

To use it, you should download the "code" or the .py file and install certain Python packages.

pip install praw <br>
pip install pandas <br>
pip install tqdm <br>

<h1>The file extracted</h1>
Since the most important aspect is the file extracted with the comments, it's crucial to know what information is contained in this file and how to open it.<br>
The file is a CSV where the separator is a tab, denoted as \t.<br>
<br>
In this file, you will find the following data:<br>
<br>
<b>Author</b> - The creator of the comment,<br>
<b>Comment</b> - The comment in its entirety,<br>
<b>Score</b> - Number of votes (which represents the total value difference between upvotes and downvotes),<br>
<b>Length</b> - Word count of the comment,<br>
<b>Parent</b> - comment refers to the ID of the comment or post to which the comment is replying,<br>
<b>Post Permalink</b> - The direct link to the post,<br>
<b>Post URL</b> - the image of the post, if it exists,<br>
<b>Permalink</b> - the direct link to the individual comment.<br>
And a few more things..<br>
<br>

<h1>How to use</h1><br>
Firstly, the reddit.py file must be in the same location as the praw.ini file. Before running the script, you should edit the praw.ini file with all the details obtained from the Reddit API. This tool will create a new folder named 'Comments' where it will save the extracted files. <i></i>It's as simple as that.</i>


<h1>Citation</h1>
Santos, B. R. (2024). Reddit extract comment. An application for automated data extraction from Reddit. Source code and releases available at https://github.com/DKZPT/Reddit-extract-comment.

<h1>Licence</h1>

Copyright (c) 2024 Rui Bruno Santos

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "code"), to deal in the software without restriction, including, without limitation, the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software, and to permit persons to whom the software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the software.

The software is provided "as is," without any warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and noninfringement. In no event shall the authors or copyright holders be liable for any claims, damages, or other liabilities, whether in an action of contract, tort, or otherwise, arising from, out of, or in connection with the software or the use or other dealings in the software.
