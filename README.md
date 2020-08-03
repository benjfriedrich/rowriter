# RoWriter()

CSS is not great at making aesthetic pleasing rows. If you put a list of items into a flex-box, it will cram as many into the first line as possible, pushing what ever leftovers there are to the second row. So if there were space for 12 items per row and you put 13 items in, it would display a row of 12 items and a row of 1 item. This isn’t good.

A better outcome in most situations would be a row of 7 items and a row of 6 items. You want as few rows as possible, and for those rows to be as even as possible.

RoWriter is a Javascript function that helps solve this problem by parsing a list of items into even rows.

RoWriter takes two arguments: 1) an array of items, and 2) a maxWidth, and it returns an array of those items parsed into subarrays that represent each row.

	RoWrite([...array], maxWidth)

Example input:
	RoWrite([a,b,c,d,e], 4)

Expected output:
	[[a,b,c],[d,e]]

[Find more here][https://rowriter.dev]
