The XSpellCheck is a React-based application designed for real-time spell-checking and auto-correction. It uses a custom dictionary to identify and suggest corrections for common typos and misspellings in user-entered text. The app focuses on improving user-written content by flagging the first detected misspelling and offering a correction.

We already have the class-component based implementation, you must convert it into functional-component based implementation without changing its UI look and working.

Here’s the dictionary that you must use. The spell-checks will be done on the basis of this.

const customDictionary = {

teh: "the",

wrok: "work",

fot: "for",

exampl: "example"

};

Upon initial render:

If we type wrong spelling for any of ther words mentioned in our dictionary, we must get a correction message. For example, when we type "wrok" in the textbox, we get the following correction suggestion:

It must work even when we enter a sentence. If there are multiple wrong spellings, it must show the correction suggestion for the first one. For example, when we type "For exampl this wrok", we get the following correction suggestion for just the first wrong spelling i.e. example for exampl:

It must be case-insensitive. For example, it must give correction suggestion the for the as well as The:

If you remove all the characters from the textbox, you must see no suggestions just like the initial render:


vercel - [xspellcheck-six-xi.vercel.app](https://xspellcheck-six-xi.vercel.app/)
