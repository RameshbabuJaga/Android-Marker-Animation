# Screencapture and animated gifs

> I say "animated gif" but in reality I think it's irresponsible to be serving "real" GIF files to people now. You should be serving gfy's, gifv's, webm, mp4s, whatever. They're a fraction of the filesize making it easier for you to deliver high fidelity, full color animation very quickly, especially on bad mobile connections. (But I suppose if you're just doing this for small audiences (like bug reporting), then [LICEcap](http://www.cockos.com/licecap/) is a good solution).

## Capturing (Easy)

1. Launch quicktime player
1. do Screen recording

![screen shot 2014-10-22 at 11 16 23 am](https://cloud.githubusercontent.com/assets/39191/4741576/9745687c-5a17-11e4-8940-b47b4f9c52be.png)

1. hit the button

![image](https://cloud.githubusercontent.com/assets/39191/4741609/e2faf96c-5a17-11e4-8c0b-3ac022c64502.png)

1. you can chose to record entire screen or a portion by dragging:
1. do that then record and hit the stop button in the top taskbar. 
  * You can then Trim the video in quicktime with `cmd-t`. 
1. File > "Save…". Save that shit.

## Capturing (Pro)

1. Use [Screenflow](http://www.telestream.net/screenflow/overview.htm). It can do 60fps and do all sorts of annotations beyond the basic clicks that Quicktime will capture.


## Making an animated gif (easy)

1. Go to [gfycat](http://gfycat.com/) and drag your mov file onto it.
![image](https://cloud.githubusercontent.com/assets/39191/4741723/30115aba-5a19-11e4-9975-f000639982f8.png)
1. get the embed code and **use the iframe**

<a href="http://gfycat.com/WeeGrizzledFruitbat">
![2014-10-22 11_35_09](https://cloud.githubusercontent.com/assets/39191/4741874/9890757a-5a1a-11e4-9a71-3f64bd66b7ab.gif)
</a>

Really, use the iframe. It'll give you better perf and will load way faster for your users.

If you really want a GIF file (terrible), then click the "GIF" icon. It's sweet to let them do the work for us.

<hr>

However if you want to make the gif on your own.. continue.


## Making an animated gif (cheater)

Use an app called [GIFBrewery](http://gifbrewery.com/) but it costs money and is a little weird to configure. But it works. Run it through [imageoptim](https://imageoptim.com/) after.


## Making an animated gif (pro)

(This path is for people comfortable with homebrew and dotfiles.)

1. Grab `gifify` from @SlexAxton's gist: https://gist.github.com/SlexAxton/4989674 and toss it into your dotfiles somewhre
2. Make sure you have the dependencies: `brew install ffmpeg gifsicle imagemagick`
3. Run it with `gifify yourvideo.mov --good`
3. Run the image through [imageoptim](https://imageoptim.com/) after.
