#twitter-bootstrap DocPad skeleton

This is a simple skeleton designed to get you up and running with [DocPad](https://github.com/bevry/docpad/) and [Twitter Bootstrap](http://twitter.github.com/bootstrap/) (compiled dynamically via [docpad-plugin-less](https://npmjs.org/package/docpad-plugin-less) so that you can override colours or spacings as you please).

The easiest way to work with this skeleton is to clone it from github and then run the relevant commands to pull down required dependencies. This doesn't require you to download or install DocPad directly (it gets pulled in locally by npm) but does have certain dependencies:

 * Git - I'll assume you already have this or can find and install it yourself.
 * Node and npm - I installed both using the [installer](http://nodejs.org/download/) from the node site.

Once you have these installed just run the following commands (starting in a sensible directory and changing `website-name` to whatever you like):

```bash
git clone git://github.com/vitch/twitter-bootstrap-skeleton.docpad.git website-name
cd website-name
git submodule update --init --recursive
npm install
node node_modules/docpad/bin/docpad install
```

Then to run the website all you need to do is:

```bash
node node_modules/docpad/bin/docpad run
```

You can call put `help` on the end of the previous command rather than `run` if you want to see the other DocPad commands you can run.

Once DocPad is running you can visit http://localhost:9778/ to see your brand new website. Changes made to files will be magically pushed to the browser without you even needing to reload. When you are finished you can `Ctrl+c` in your terminal window to stop DocPad from running.

To distribute your site run:

```bash
node node_modules/docpad/bin/docpad clean
node node_modules/docpad/bin/docpad generate
```

And your `out/` directory will contain the static files which make up your site and can be uploaded to any server.