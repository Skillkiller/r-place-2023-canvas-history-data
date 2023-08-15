# r/place 2023 Data
> Posted by u/arbeitrary

You all have shared your creativity and passion with us through another r/place adventure. We once again share some of the data with you.

## Media
Full-frame canvas prior to whiteout: https://placedata.reddit.com/data/final_2023_place.png

And higher-resolution versions, just in case:
- https://placedata.reddit.com/data/final_2023_place_2x.png
- https://placedata.reddit.com/data/final_2023_place_4x.png
- https://placedata.reddit.com/data/final_2023_place_8x.png

But you and I know that the canvas is not a snapshot. It lived and breathed, until we smothered it with white pixels. You can see its lifecycle here: [Official canvas timelapse: r/place 2023](https://www.reddit.com/r/place/comments/15ackvw/official_canvas_timelapse_rplace_2023/)

## Canvas activity data
You can find the full timeline of activity as a set of CSV files with the following columns: ``timestamp``, ``user``, ``coordinate``, ``pixel_color``
- timestamp: the UTC time for the pixel-placement
- user: obfuscated identifier for the user taking this action. These are consistent within the dataset, so you can see how users behaved across the canvas and timeline. But they are not Reddit user IDs (and don’t match the IDs from last year’s data).
- coordinate: the location of this placement. This year we have negative coordinates, so that “0,0” is the approximate center of the canvas.
- pixel_color: the hex color code for the pixel

You will also find coordinates that don’t match a simple “x,y” pattern. In the case of 4 simple coordinates (“x1,y1,x2,y2”), these correspond to the upper left x1, y1 coordinate and the lower right x2, y2 coordinate of a moderation rectangle. We also have values that look like “{X: 424, Y: 336, R: 3}”, which specify a moderation circle with a center at the “X” and “Y” values and a radius of the “R” value.

We have split the data into 53 gzipped CSV files: https://placedata.reddit.com/data/canvas-history/2023/2023_place_canvas_history-000000000000.csv.gzip through https://placedata.reddit.com/data/canvas-history/2023/2023_place_canvas_history-000000000052.csv.gzip.

You can find the whole list here: https://placedata.reddit.com/data/canvas-history/2023/index.html

I look forward to seeing what our users create from this output of their own creation.