# Cardiology

## README
Inspired by a [Wired article](https://www.wired.com/2010/11/ff_bloodwork/3/), which showcased a redesign by David McCandless of the standard "Blood Work Cardiology Result" report. 

Built this to implement David's dataviz using d3.js. So, here goes - this simple app was built using:

1. Twitter's Bootstrap: http://getbootstrap.com/.
2. Mike Bostock's "d3.js": https://github.com/mbostock/d3.
3. JQuery: https://jquery.com/.

## INSTRUCTIONS
1. Open the shell and unzip the archive
$ cd ~
$ unzip cardiology.zip

2. Change to root directory:
$ cd cardiology

3. Start server from this root directory:
$ python -m SimpleHTTPServer 8080

4. Launch browser and hit http://localhost:8080/.

## DEMO
Screen recording of the demo is under "docs" directory: cardiology_screen_recording.mov.

## DATA
The data for the 3 demo patients (carl, carol & frank) are sourced from the corresponding "json" files:
```
├── bullet_carl_lee.json
├── bullet_carol_allen.json
├── bullet_frank_taylor.json
```

For instance, frank's json looks like this:
```javascript
[
  {"title":"CRP level test","subtitle":"mg/L","ranges":[1,3,10],"measures":[0.6],"markers":[0.6]},
  {"title":"Total cholesterol","subtitle":"mg/dL","ranges":[200,239,320],"measures":[141],"markers":[141]},
  {"title":"LDL cholesterol","subtitle":"bad cholesterol (mg/dL)","ranges":[159,189,300],"measures":[102],"markers":[102]},
  {"title":"HDL cholesterol","subtitle":"good cholesteror (mg/dL)","ranges":[100,129,159],"measures":[39],"markers":[39]}
]
```

"ranges" may not need a change unless you think otherwise. To show a wider difference, modify "measures" & "markers" (both are to be the same, in order to avoid confusion in this specific usecase).

To learn more about this particular graph and how to modify values: http://bl.ocks.org/mbostock/4061961.

## CONTENTS
```
├── about.html
├── bullet.js
├── bullet_carl_lee.html
├── bullet_carl_lee.json
├── bullet_carol_allen.html
├── bullet_carol_allen.json
├── bullet_frank_taylor.html
├── bullet_frank_taylor.json
├── cardiology.sublime-project
├── cardiology.sublime-workspace
├── carol_allen.html
├── docs
│   ├── cardiology_screen_recording.mov
│   └── readme.txt
├── frank_taylor.html
├── index.html
└── static
    ├── bootstrap-3.3.2-dist
    │   ├── css
    │   │   ├── bootstrap-theme.css
    │   │   ├── bootstrap-theme.css.map
    │   │   ├── bootstrap-theme.min.css
    │   │   ├── bootstrap.css
    │   │   ├── bootstrap.css.map
    │   │   └── bootstrap.min.css
    │   ├── fonts
    │   │   ├── glyphicons-halflings-regular.eot
    │   │   ├── glyphicons-halflings-regular.svg
    │   │   ├── glyphicons-halflings-regular.ttf
    │   │   ├── glyphicons-halflings-regular.woff
    │   │   └── glyphicons-halflings-regular.woff2
    │   └── js
    │       ├── bootstrap.js
    │       ├── bootstrap.min.js
    │       └── npm.js
    ├── bootstrap-3.3.2-dist.zip
    └── custom
        └── css
            └── navbar.css
```
