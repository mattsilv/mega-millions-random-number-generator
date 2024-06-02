# Mega Millions Random Number Generator

This repository contains a simple web-based tool that generates Mega Millions lottery numbers using true randomness from [RANDOM.ORG](https://www.random.org/). The tool is built with HTML, CSS, and JavaScript, and it uses the [Axios](https://github.com/axios/axios) library for making HTTP requests.

## Demo

Check out the live demo of this tool in the blog post: [Are Online Lotto Ticket "Auto Fill" Numbers Truly Random?](https://silv.blog/are-online-lotto-ticket-auto-fill-numbers-truly-random/)

## How It Works

The main functionality of the tool is implemented in the `index.html` file. When the "Generate Mega Millions Numbers" button is clicked, the tool:

1. Fetches 5 unique main numbers (1-70) from RANDOM.ORG using the Axios library.
2. Fetches 1 Mega Ball number (1-25) from RANDOM.ORG.
3. Displays the generated numbers on the page in a visually appealing format.
4. Enforces a waiting period of 15 seconds before allowing another set of numbers to be generated.

The tool adheres to RANDOM.ORG's guidelines by providing an email address in the `User-Agent` header of the HTTP requests and implementing a timeout to allow the server sufficient time to fulfill the requests.

## Usage

To use this tool locally, simply clone the repository and open the `index.html` file in your web browser.

```bash
git clone https://github.com/mattsilv/mega-millions-random-number-generator.git
cd mega-millions-random-number-generator
open index.html
