# Customer Retention Prediction
TL;DR
(project goal, context, data, model, result)

# Introduction

## Motivation
- A key to a company's growth is its **ability to keep customers** 
  - Keeping existing customers is more cost efficient than acquiring new ones
  - It speaks about brand attractiveness and customer experience 
- In the context of e-commerce, i.e., non-subscription based business, customer retention = **repeated visits from the same customer**
  -  Relevant questions to ask are how far apart visits need to be for a user to be considered as a returning user, and what events should be deemed as _visits_
  -  It is worth noting that the answers to these questions, and even the definition of customer retention, can vary across businesses
- Knowing if a customer will return is valuable
  - Help to distinguish different types of shoppers and understand their needs
  - Allow preemptive measures to prevent churns
  - An effective way to evaluate if a marketing campaign or a sale event is successful

## Case background
- The subject of study is an online retailer of multi-category consumer goods with a pseudonym *PrimeBuy*
- Primary data is user activities on *PrimeBuy* 
  - Collected by [Open CDP](https://rees46.com/en/open-cdp) project and available on [Kaggle](https://www.kaggle.com/mkechinov/ecommerce-behavior-data-from-multi-category-store)
  - More details to be discussed below
- Focal interests of study
  - How to measure customer retention of PrimeBuy
  - What can user activities tell about retention
  - Any value-adding opportunities and strategies

## Data
- Activity level data with each row representing a user's activity (such as view) on a certain product and the corresponding timestamp
- Restricted to user activities between Oct 2019 and Mar 2020. 286 million rows (44GB+)
- Nine columns:
  - *Event_time*: Timestamp of a user activity in UTC
  - *Event_type*: Type of activities. Either view, cart, or purchase. About 94% are view, 4% cart and 2% purchase
  - *Product_id*: Unique identifier of a product
  - *Category_id*: Unique identifier of a category of products
  - *Category_code*: Category name if available. About 24% are missing, 16% smartphone
  - *Brand*: Brand name of a product if available. About 13% are missing
  - *Price*: Product price. Average product price is $174
  - *User_id*: Unique identifier of a user
  - *User_session*: Temporary user session ID. Will change whenever users switch devices, log off and on, or have a long pause in activities

![Data screenshot](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "PrimeBuy user activity data")





## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/yz-joy/user-retention/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/yz-joy/user-retention/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
