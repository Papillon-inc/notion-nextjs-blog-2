# A Next.js, Notion API and Tailwind CSS starter blog template 

This is an open-source starter blog template that is statically generated with Next.js, content powered by the Notion API, styled with Tailwind CSS and deployed with Vercel.

*Still a work in progress.*

**Live example hosted on Vercel**: 

## Getting Started

1. Clone this repo `git clone https://github.com/luciovilla/notion-nextjs-blog.git`
2. Install its dependencies `npm install`
3. Copy or rename the `.env.example` file to `.env.local`
4. Personalize the page meta data in `Container.js`

## Creating Your Notion Pages Table

1. Create a blank page in Notion
2. Create a table on that page.
3. Add the following columns to the table:
- `Page` (type: title): this the blog post's headline and meta title.
- `Slug` (text): this is the blog post's URL slug.
- `Date` (date): the display date and meta published_time property.
- `Description` (text): this is the preview text on the homepage and the meta description property.

View this sample template table in [Notion](https://www.notion.so/8dde3326f8cb4cc68b47a96bea86e9be).

## Getting Database ID and Notion Token

- Create a [Notion Integration](https://www.notion.so/my-integrations).
- Copy and paste the Integration Token in the `.env.local` file: `NOTION_TOKEN=____`
- On the Notion page, click the "Share" button in the top right and  share the database with the Notion Integration you just created
- In a browser, go to the Notion page and grab the Database ID from the URL. Its the part of the URL after your workspace name and the slash and before the question mark. The ID is 32 characters long, containing numbers and letters.
- Paste your Database ID in the `.env.local` file: `NOTION_DATABASE_ID=___`

## Creating Blog Posts

1. In Notion click new on the table to add a new row
2. Fill in the Page title, Slug, Date and Description
3. Keep the Description text short, as it will be the text that shows up on the homepage as the post's preview text.

## Running Locally

Run `npm run dev`

## Credits
Tk Tk