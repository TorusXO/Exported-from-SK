# Library of exported Spiral Knights models
 This repo contains original files of sk with their converted versions.

 All of the models that were able to convert are put in their .dat s folders with .glb extensions. 

 Most of the .dat files are from the game files that may be found in rsrc folder. 

Every file possible to convert was converted, some of these files could still be converted, but contain 0 meshes. Such files aren't included

Also there are some .blend files that I made during the exploration of the files, feel free to use them.
If there are some files that weren't exported (and they can be exported)- please let me know in the Issues section 
#### why do I need this repo?
I wanted to make fanarts of the game, that's why I had to export whole folders at once. 
Now I'm sharing it with you, so that there could be more 3D arts or animations of our beloved game.

## How to copy this large repo:
You need to add a few adjustments to .gitconfig that is global to your system.

Open system console and write:

```commandline
git config --global core.compression 0
```

For windows you will need to locate the .getconfig file in the system root folder

To locate and edit the .gitconfig file on macOS, you can follow these steps:

1. Open the Terminal application, which is usually found in the "Utilities" folder within the "Applications" folder.

2. Type `cd ~` and press Enter to navigate to your home directory.

3. Run `ls -la` to display all the files, including hidden files, in your home directory.

4. Look for the `.gitconfig` file. If it exists, use a text editor to open it by running: `open -e .gitconfig`.

5. If the `.gitconfig` file does not exist, you can create it by running: `touch .gitconfig` and then open it using a text editor with the command from step 4.

6. Once the file is open in the text editor, add the following lines:

```
[core]
    packedGitLimit = 512m
    packedGitWindowSize = 512m
[pack]
    deltaCacheSize = 2047m
    packSizeLimit = 2047m
    windowMemory = 2047m
```

7. Save the changes and close the text editor.

Then add to the command line:

```commandline
git clone --depth 1 <repo_URL>
```
if it works then use github desktop to pull all the files to the local git or run the following:
```commandline
git fetch --unshallow 

or, alternately,

git fetch --depth=2147483647

Now, do a regular pull:

git pull --all

```
