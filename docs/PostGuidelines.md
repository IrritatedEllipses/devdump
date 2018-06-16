# Design Notes for Dev Dump

## Description of Dev Dump

Dev Dump is a daily thread on the Shacknews Chatty ( <http://www.shacknews.com/chatty> ) where Developers of all types can come together to ask questions, talk about their developer experiences, discuss current events in the development world, and learn from each other. Dev Dump is an all inclusive discussion for developers of all skill levels, whether retired from a life long career of creating or merely just interested in making "Hello, World!" appear on the screen for the very first time.
***

## Structure of normal Daily Dev Dump

Daily Dev Dump should begin with either two or three posts:

1. Dev Dump Main Header.
2. Dev Dump Discussion Articles.
3. (optional) Extra Dev Dump Post.

### Dev Dump Main Header

The main header should include the date of the current thread in "Month, day year" format followed by "b{Dev Dump}b", a line break, and a short, humorous comic about the development world. Comics should be SFW, inoffensive and, although poking fun at a language or group of developers is permissable, the following common sense guidelines apply:

* No comics that make fun of race, gender, orientation, sexual identity, or disability (Excluding PHP) are permissible.
* Language must be kept PG-13 or lower.
* No nudity or realistic violence allowed.
* No drugs outside of nicotine and alcohol should be explicitly mentioned or shown.
* No Rick Rolls.
* No excessive series of jokes (Driving a point into the ground). If a comic involving the same subject is topically poignant (such as Microsoft acquiring GitHub in 2018-06) no more than two comics in a row, and three in a week should reference the subject.

To provide a clean Shacknews Chatty nothing else should be listed in the main header.

### Dev Dump Discussion Articles

The second post should begin with "g{Links you've already clicked}g" followed by a short selection of recent articles concerning the development world. The structure of the articles should start with the title of the article, a line break, the URL of the article, two line breaks, and a short synopsis of the article as read by the creator of that days Dev Dump followed by three line breaks. For example:

        A Dev Dump Example  
        http://www.example.com/devdumpexample  

        This is an example of a Dev Dump article and I find it fascinating because it shows me how to write Dev Dumps!
Discussions articles must follow the same common sense guidelines as main header comics, though special dispensation should be allowed for artistic expression within the articles. Synopses of the articles should be insightful, on topic, and include a reason - implicit or implied - why that particular article was posted.

No article posted should explicitly require payment, subscription, or membership to any company or website to read. Any article that prompts for a sign up that can be easily dismissed or shows an ad that cannot be skipped (such as a YouTube advertisement) are permissable.

Although sales and deals on items (such as book sales, online courses or tooling sales) may be included within the discussion articles no referral links that benefit Dev Dump, partners of Dev Dump, or people personally known to Dev Dump may be used in the Dev Dump Article Discussion. If a referral link will be used that referral link should go into the (Optional) Extra Dev Dump Post.

Articles written by persons known to Dev Dump will be permitted even if there are advertisements within the article, as long as the relationship between Dev Dump and the articles author is made explicit.

### (Optional) Extra Dev Dump Post

After these two posts if there is any news about Dev Dump itself, or additional sections that should be added, each section should start with a green tag (g{    }g) and a subject heading for that section. So as not to interrupt the normal flow of the Shacknews Chatty no more than three main heading posts should be entered in the daily Dev Dump.

Referral links that benefit Dev Dump, partners of Dev Dump, or people personally known to Dev Dump may be included in this section of Dev Dump as long as:

* The link is surrounded above and below with the red tag (r{    }r) and the words "REFERRAL LINK". For example:

        r{REFERRAL LINK}r
        http://www.example.com/referral-link-give-me-money&_please
        r{REFERRAL LINK}r

* A non referral link is provided plainly and visibly within the body of the article.

## Dev Dump Header Snippet

The following is a snippet in JSON for Visual Studio Code which can be used in the user added Markdown section to help guide how the Dev Dump should be formatted:

```javascript
"Dev Dump Template": {

        "prefix": "devd",
        "body": [
                "### $CURRENT_DAY_NAME, $CURRENT_MONTH_NAME $CURRENT_DATE, $CURRENT_YEAR b{DEV DUMP}b",
                "",
                "<$1>",
                "",
                "## g{Links you've already Clicked}g",
                "",
                "### $0"

        ],
        "description": "Dev Dump heading"
},
```