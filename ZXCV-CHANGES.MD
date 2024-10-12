Only tested on 4.3.9
I am not a coder, all changes made by googling then fiddling around and seeing what worked
In an acceptable state for my use case, will not be making further changes

all changes made in the following file
nightwalker.css

located at nightwalker-zxcv\private\css\nightwalker.css

1.	Added new Line 13 --color-Yellow: #d1c52a;
		All lines below shifted down 1 from original nightwalker-main as a result

2. 	Changed Line 47 from
		color: var(--color-White) !important;
	to
		color: var(--color-Yellow) !important;
	This makes hyperlinks stand out

3. Line 439
		display: inline;
	to
		display: block;
	This makes the entire line clickable on the Status filters
	But makes the filters be split out into 2 lines. 1 with the unclickable custom icon and 1 with the clickable text
	This is band-aid fixed in change 4.

4. Commented out the Custom Icons content items in the following lines
		449, 464, 479, 494, 509, 524, 539, 554, 569, 584, 599, 614
	This removes the custom icons but gets the Status filters back down to 1 Line
	
5. Added the original icons back by making the following change
		display: none;
	to
		display: inline-block;
	On the following lines
		443, 458, 473, 488, 503, 518, 533, 548, 563, 578, 593, 608
		

