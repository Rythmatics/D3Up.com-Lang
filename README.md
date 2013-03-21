D3Up.com-Lang
=============

This GitHub repository contains the Language Files used for D3Up.com.

Want to help translate D3Up.com into more languages?
---

Then you're in the right place. This repository contains all of the language files used on the website and anyone can contribute to it's modification. I will be updating this documentation to clarify the process as I find better ways to explain it. 

Getting Started
---

If you're not familiar with Github and Pull Requests, here's a basic step by step guide on how you can contribute!

**Step #1 - GitHub Account**

First off, you'll need a GitHub account, which you can [register for here](https://github.com/signup/free).

**Step #2 - Fork the Language Repository**

Next up, you'll need to create a copy of the repository that you can edit. This is called "Forking", which basically creates a copy of everything that you're free to edit and modify.

Head on over to the primary repo, located at [https://github.com/aaroncox/D3Up.com-Lang](https://github.com/aaroncox/D3Up.com-Lang) and in the upper right, you'll see a 'Fork' button. Go ahead and click it. 

You'll now notice that you have your own Repo, that will be located on GitHub on /(username)/D3Up.com-Lang, and you'll automatically be redirected to it. It will now also show up on your GitHub dashboard under "Your Repositories" for future reference. 

**Step #3 - You're all setup!**

For the most basic setup, using GitHub to edit the files, just browse through the folders and click on the file you wish to edit. At the top, you'll notice there's an edit button, you can use that to edit the files directly on GitHub. 

If you're familiar with GitHub, you're free to clone these files down onto your local machine as well to make edits with your favorite text editor. [This help page](https://help.github.com/articles/fork-a-repo) on GitHub explains a bit more on the commands and how to update your files from my repo. 

**The Language File Structure**

The language files at their most basic level look like this:

```php
<?php
	<?php
	return array(
		'key1' => 'value1',
		'key2' => 'value2',
	);
?>
```

If you are not familiar with programming, these files may look a bit strange. Basically, the 'key' part of the file is what I use on the site to place the translated terms, and the 'value' part is the text it shows for the language the user picks. So for example, in the `/en/build.php` file, we have:

```php
<?php
	<?php
	return array(
		'build' => 'Build',
	);
?>
```

In english, I've been calling the 'Character Builds' just 'Builds'. However, in another language, it might be better to describe them as something else. I've implemented a *Pig Latin* language file, located under the `/pl` folder. If you look at the `/pl/build.php` file, it looks like this:

```php
<?php
	<?php
	return array(
		'build' => 'Uild-bay',
	);
?>
```

All you have to do is change the 'value' side of the code to what it should be called in the language you're working with. 

If you'd like to **start a new language**, feel free to copy the `en` folder and make a new folder, with a 2 letter abbreviation of the language you want to create, then start modifying!

**Step #4 - Submitting your changes via a Pull Request**

When you've modified some files and would like them put into D3Up, this is when you'd issue a pull request. 

On the top of the page on GitHub, on your "Forked" repository, there is a "Pull Request" button. If you click that, it will bring you to a form with a Title and a spot for a message. 

Please fill out the fields as follows:

- Title: What language you're making changes in, and maybe what section of the site the changes are for 
- Body: A written description of what you've done, any comments you may have and any other information you deem relevant. 

Then just hit Send Pull Request, and it will notify me that you've made changes you'd like approved for D3Up. It will also bring you to a page that looks much like a forum post, where anyone can comment and have a discussion about the changes you just made. I may leave some comments if something seems wrong, or I may ask you to change things to fit with the standards needed for the code. Once everything is good, I'll approve it and your changes will make their way into D3Up.com's language files!

Questions? Feel free to head on over to the "Issues" section of the D3Up repository and post or you can email me, my emails on the top of all the pages of D3Up!

Thanks for helping translate D3Up into many other languages!