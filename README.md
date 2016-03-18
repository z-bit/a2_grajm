# Basic Seed with ng2-material
## Based on [Rob Wormald](https://gist.github.com/robwormald/429e01c6d802767441ec) and [Justin Dujardin](https://justindujardin.github.io/ng2-material/)
<pre><code>
$ git clone https://github.com/z-bit/a2seed-rob_jspm.git a2seed_rob_mat
$ npm install 
$ jspm install 
</code></pre>
* run code with live-server ==> **works**

<pre><code>
$ jspm install npm:ng2-material
$ jspm install css

@create /src/app.scss:
    $md-font-url: "../jspm_packages/npm/ng2-material@0.2.10/dist/";
    @import "../jspm_packages/npm/ng2-material@0.2.10/dist/font";
    @import "../jspm_packages/npm/ng2-material@0.2.10/source/all";

$ sass rc/app.sss src/app.css

@edit /src/app.ts: 
    import {MATERIAL_DIRECTIVES, MATERIAL_PROVIDERS} from "ng2-material/all";
    import './app.css!';
    ...
    @Component({
        **directives: [MATERIAL_DIRECTIVES],**
    ...       
</code></pre>

* @edit app.html: 
    * copy source code from [ng2-material Demo Page - Buttons](https://justindujardin.github.io/ng2-material/#/components/button) 
   
* run with live-server => **OK**
