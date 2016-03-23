# a2_grajm 
### Angular 2 Seed with Gulp, Redux, Angular2, JSPM, Material Design
#### Based on [Rob Wormald](https://gist.github.com/robwormald/429e01c6d802767441ec) and [Justin Dujardin](https://justindujardin.github.io/ng2-material/) and [Gerard Sans](https://medium.com/google-developer-experts/angular-2-introduction-to-redux-1cf18af27e6e#.dj3aclq7s)
Version 0.01

<pre><code>
$ git clone https://github.com/z-bit/a2_grajm.git my_app
$ cd my_app
$ npm install 
$ jspm install 
</code></pre>

* to update the quickly developing libraries

<pre><code>
$ jspm install angular2          //problems with angular2@2.0.0-beta.11 (beta.9 fine)
$ jspm install npm:ng2-material  //now: ng2-material@0.2.12
$ jspm install npm:redux
</code></pre>
### unsolved problem
* /app/app.scss is manually compiled
    * `cd app`
    * `sass app.scss spp.css`
* this worked in the beginning
* in between there must be a config stating that /app is the root
* now the urls in the app.css are rerouted `../jsmp_packages => /app/jspm_packages`
* quickfix: `./../` in app.scss which will be edited (after translation) in app.css: `./../ => ../..` (works)


* run code with live-server ==> **works**
