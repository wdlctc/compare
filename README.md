
- **folder1/** and **folder2/** each contain five videos named `video1.mp4` through `video5.mp4`.
- **index.html** renders them in a 2-column grid for visual comparison.

## Usage

1. Clone or download this repo.  
2. Put your MP4 videos into `folder1/` and `folder2/` with matching names.  
3. Open `index.html` in any modern browser.

## index.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Two-Column Video Gallery</title>
  <style>
    body {
      font-family: sans-serif;
      margin: 20px;
    }
    .video-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-auto-rows: auto;
      gap: 20px;
    }
    .video-grid video {
      width: 100%;
      height: auto;
      display: block;
    }
    .video-grid .title {
      text-align: center;
      margin-bottom: 8px;
      font-size: 0.9em;
      color: #333;
    }
  </style>
</head>
<body>

  <h1>Video Comparison</h1>
  <div class="video-grid">
    <!-- Row 1 -->
    <div>
      <div class="title">Video 1 (Folder 1)</div>
      <video controls src="raw/A movie trailer featuring the adventures of the 30 year old space man wearing a red wool knitted mot-0.mp4"></video>
    </div>
    <div>
      <div class="title">Video 1 (Folder 2)</div>
      <video controls src="test/A movie trailer featuring the adventures of the 30 year old space man wearing a red wool knitted mot-0.mp4"></video>
    </div>
    <!-- Row 2 -->
    <div>
      <div class="title">Video 2 (Folder 1)</div>
      <video controls src="raw/A stylish woman walks down a Tokyo street filled with warm glowing neon and animated city signage. S-0.mp4"></video>
    </div>
    <div>
      <div class="title">Video 2 (Folder 2)</div>
      <video controls src="test/A stylish woman walks down a Tokyo street filled with warm glowing neon and animated city signage. S-0.mp4"></video>
    </div>
    <!-- Row 3 -->
    <div>
      <div class="title">Video 3 (Folder 1)</div>
      <video controls src="raw/Animated scene features a close-up of a short fluffy monster kneeling beside a melting red candle. T-0.mp4"></video>
    </div>
    <div>
      <div class="title">Video 3 (Folder 2)</div>
      <video controls src="test/Animated scene features a close-up of a short fluffy monster kneeling beside a melting red candle. T-0.mp4"></video>
    </div>
    <!-- Row 4 -->
    <div>
      <div class="title">Video 4 (Folder 1)</div>
      <video controls src="raw/Drone view of waves crashing against the rugged cliffs along Big Sur’s garay point beach. The crashi-0.mp4"></video>
    </div>
    <div>
      <div class="title">Video 4 (Folder 2)</div>
      <video controls src="test/Drone view of waves crashing against the rugged cliffs along Big Sur’s garay point beach. The crashi-0.mp4"></video>
    </div>
    <!-- Row 5 -->
    <div>
      <div class="title">Video 5 (Folder 1)</div>
      <video controls src="raw/Several giant wooly mammoths approach treading through a snowy meadow, their long wooly fur lightly -0.mp4"></video>
    </div>
    <div>
      <div class="title">Video 5 (Folder 2)</div>
      <video controls src="test/Several giant wooly mammoths approach treading through a snowy meadow, their long wooly fur lightly -0.mp4"></video>
    </div>
  </div>

</body>
</html>
