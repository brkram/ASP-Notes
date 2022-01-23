# 67656 Advanced Signal Processing- Lecture Notes


My lectures notes for 67656: Advanced Signal Processing
at Hebrew University of Jerusalem Israel (HUJI), in Hebrew.

To access the notes, you should install
* [git](http://git-scm.com/book/en/Getting-Started-Installing-Git)
* [LyX - Yair's guide](http://bit.ly/LYXGuide). If you are new to
LyX, then welcome to the community :)

I strongly recommend watching [David Zisselman's](https://www.youtube.com/watch?v=bEmeWkR4IXc) tutorial on how to start using LyX...
If you wish to contribute to the notes, you will need to configure git to
[authenticate with Github](https://help.github.com/articles/set-up-git#next-steps-authenticating-to-github-from-git)
and follow the steps below.

## Access

To pull the notes to your local computer you must first `clone` the repository.
In the terminal, navigate to the root directory where you'd like the notes to
be located and enter:

```sh
git clone https://github.com/brkram/ASP-Notes.git
cd ASP-Notes
```

You will see a directory containing some pictures from the lectures, the lyx file containing the lecture notes, a macro file and a compiled version (pdf) of my notes.

If one updates the notes, you can pull down the newest changes by
executing the following command in the notes directory:
```sh
git pull origin main
```


## Contribute


If you'd like to make changes to the notes, you will have to do so in your own
repository and create a [pull request](https://help.github.com/articles/using-pull-requests). 
First, you need to `fork` the repository on Github. 

- Navigate to the [repository page](https://github.com/brkram/ASP-Notes.git)
- Click the fork button and follow the instructions ![fork
    button](https://github-images.s3.amazonaws.com/help/repository/fork_button.jpg)
- In the terminal, navigate to the root directory where you wish to store the
    notes
- Clone the forked repo locally
```sh
git clone https://github.com/YOUR_USERNAME/ASP-Notes.git 67656-lecture-notes-fork
cd 67656-lecture-notes-fork
git remote add upstream https://github.com/brkram/ASP-Notes.git
```

- Make changes to relevant section
- Compile your changes and make sure they look correct
- Commit your local changes
```sh
git add -A .
git commit -m "A SUMMARY OF YOUR CHANGES"
```

- Sync your repo with upstream changes (you may need to
    [fix conflicts](https://stackoverflow.com/questions/161813/fix-merge-conflicts-in-git))
```sh
git fetch upstream
git checkout main
git merge upstream/mian
```

- Once merges are done, push your changes to your remote fork on Github
```sh
git push origin main
```
       
- On the Github page for your forked repository, you can then create a pull
    request. If you are unsure how to do so, we recommend following the [Github
    tutorial](https://help.github.com/articles/using-pull-requests#before-you-begin).

### Special thanks

To [Ed Felten](https://github.com/edfelten/cos432-lecture-notes) for using his wonderful readme.md template for course notes and great instructions on how to fork and contribute.
