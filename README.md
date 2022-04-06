# unity-web3-integration
WebGL Template and examples to allow integration with blockchain Solana and Web3 extension wallets.

There is a detailed gist with all the required steps.

The gist is here:
https://gist.github.com/cobyism/4730490

From the gist
Deploying a subfolder to GitHub Pages
Sometimes you want to have a subdirectory on the master branch be the root directory of a repository’s gh-pages branch. This is useful for things like sites developed with Yeoman, or if you have a Jekyll site contained in the master branch alongside the rest of your code.

For the sake of this example, let’s pretend the subfolder containing your site is named dist.

Step 1
Remove the WwbGLTmemplates/Web3Template directory from the project’s .gitignore file 

Step 2
Make sure git knows about your subtree (the subfolder with your site).

git add WwbGLTmemplates/Web3Template && git commit -m "Initial dist subtree commit"
Step 3
Use subtree push to send it to the gh-pages branch on GitHub.

git subtree push --prefix WwbGLTmemplates/Web3Template origin gh-pages
Boom. If your folder isn’t called dist, then you’ll need to change that in each of the commands above.
