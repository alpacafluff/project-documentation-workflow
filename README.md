# Project Documentation Workflow 
*(In progress)*

This is for self-reference, in an attempt to get some order in the chaotic sea of files and uneven texts I'm stuck with. But I thought might be of use to others. My OS is in Spanish, so the screen captures will also be in Spanish. Sorry for that :/ Have tried to translate what I think the names in English are. 

This reference guide also at times refers to Adobe and Mac OS products I use to create/edit media. 

## Media 
Before using this guide you must have installed in Terminal
- Homebrew ([updated version at](https://brew.sh/))
- ffmpeg `brew install ffmpeg`

1. Take photos/videos
2. Download to computer
3. Create a new folder. Name it something like: YYYYMMDD-PROJECTNAME-preprocessed (substitute capitalized items with custom information). Make sure this folder lives (as a child) of your main (parent) project folder (YYYYMMDD-PROJECTNAME), and *ideally* inside a folder called YYYYMMDD-PROJECTNAME-media.
4. Note: try to avoid using the Desktop as the parent folder of 
your project folder and try to think of a more permanent location beforehand (AKA a folder called 'Projects' in your 'Documents' folder, or something like that).

5. Rename files in said folder (default name will look something like: IMG_8724) to the name of the folder plus number, e.g.: 2018-lunarlander-preprocessed-1, ...2, ...3
	
	To batch rename in Finder: 
	- Select all files, right click mouse and select "Rename x items"
	- Select "Format" from first drop down menu 
	- Select "Name and index" from the second drop down menu ("Name Format")
	- Select "After name" from the third drop down menu ("Location")
	- Enter "2018-lunarlander-preprocessed_" into the text box (without the quotation marks) and make sure the numbers start in 1
	- Press Enter.

### Photos
If images DON'T need editing* batch resize so they all have a width of 600px. 
1. FIRST, create a copy of the preprocessed folder. Remove the 'preprocessed bit'. 
2. In terminal type `for %%a in ("*.jpg") do ffmpeg -i vf scale=320:-1 %%a.png`

*If the images do need editing, use Lightroom to edit and output the files under a new folder and name (like the above, YYYYMMDD-PROJECTNAME, except in this case you don't create a copy beforehand, but it's created on the export). 

### Gifs
https://gfycat.com/gifbrewery
If videos DON'T need cropping (ffmpeg): 
(commands shared by Richard Lapham)



If videos need cropping, crop in iMovie (fastest way)
- Separate audio
- Crop
- Modify speed


## Text 

### Basic project template 
- Project title
- [A good shot of finished piece]
- Description
- Context/Inspiration (moodboard)
- Sketches/System diagrams (if applicable)
- Link to Github (if applicable)
- Materials and Tools 
- Process [include photos/gifs in chronological order, complemented with small blurbs in the captions]
- Resources 

### Portfolio case study template
- Project title
- Date
- [A good shot of finished piece]
- Description (short!)
- Product
- Audience
- Team/Client/Course (this field varies)
- Challenge
- Role
- Materials and Tools 
- Shared credit /Thanks
- Context (if applicable)
- Conceptualization/ Strategy (if applicable) 
- Sketches/System diagrams/User maps/Wireframes (if applicable)
- Link to Github (if applicable)
- Highlights of process (include photos/gifs in chronological order, complemented with small captions...can have different subtitles)


### Markdown
I write using markdown in iA Writer. Then I blog on a self-hosted site that uses Wordpress.ORG (Currently trying out this plugin: https://wordpress.org/plugins/wp-markdown/)

Here's the complete [Markdown reference from Github](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
