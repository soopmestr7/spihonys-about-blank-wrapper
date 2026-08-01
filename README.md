# spihony's about:blank wrapper (rainyware launcher)
this is an about:blank wrapper. if you don't know what that is it basically opens an about:blank page then embeds a site inside of an iframe. (this has one very specific purpose)

in the latest release version we made it have some hardcoded "bookmarks" that are sites you can open, and this repo's designed to help you make your own personalized version with your own bookmarks.

(btw the language thing lied it's also CSS and JS inline)

UPDATE 8/1/26: the font file it requested broke and so now this version fixes it. even though this is discontinued software doesn't mean i can't support it anymore.

anyway here's the instructions

# template
once you download the template, open it in your editor of choice. go to line 142, you will see this:
```javascript
// this is where the bookmarks go

const BOOKMARKS = [
  {
    name: "rainyware",
    desc: "your friendly neighborhood rainyware",
    url: "https://rainyware.rainsounds2.com"
  },
  {
    name: "your very own bookmark", //name of your bookmark
    desc: "it could be a boat!", //a description about it
    url: "https://example.com" //the link it goes to (should probably work in an iframe if you're gonna add it)
  } //PUT A COMMA HERE WHEN YOU ADD A BOOKMARK AFTER!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
];
```
i recomend opening the editor and a browser side-by-side (oh boy what a great day to have something like rainybrowser).

each bookmark has a name, description and URL and should look like this on a good day:

<img width="1411" height="656" alt="image" src="https://github.com/user-attachments/assets/7fd570bf-96d1-4087-8b16-c5e6e707e093" />

# adding bookmarks
the best place to start is to edit the bookmarks that are already there. i've included some helpful tips that tell you not to forget the comma after the entry.

when you need to add more bookmarks, add a comma after the closing bracket of the last bookmark, then copy paste this under it but before the closing bracket of the whole thing:
```javascript
  {
    name: "bookmark name",
    desc: "bookmark description",
    url: "https://example.com"
  }
```
once you add that and change the URL and stuff, load the file in your browser and your new bookmark should be there.

repeat this for more bookmarks (idk what the maximum is since the main version only has like 6)

# testing
now this is a very finnicky tool but it's currently the most stable and least destructive securly bypass atm so it's fine.

with that said a lot of site have their cross origin security policy set to disallow embedding inside an iframe. 

the best way to test before adding a bookmark is enter it in the URL bar before trying it as a bookmark. if it works, great. if it looks like this:

<img width="274" height="174" alt="image" src="https://github.com/user-attachments/assets/a5626716-d000-46bd-92b6-516d23393c27" /> <img width="563" height="200" alt="image" src="https://github.com/user-attachments/assets/1a773d96-f2b0-454e-b0b8-f94926c0f6b6" />

then cross origin embedding doesn't work and so it won't work.

# none of the bookmarks show up at all when i add one, what do i do?
<img width="723" height="461" alt="image" src="https://github.com/user-attachments/assets/27e0d2de-13be-48b9-8b3e-22d1330d8908" />




