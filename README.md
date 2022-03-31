# Codebase Cleanup

To get started with the ["Codebase Cleanup" Exercise](https://github.com/prof-rossetti/intro-to-python/blob/main/exercises/codebase-cleanup/README.md).

## Setup

Create and activate a new virtual environment:

```sh
conda create -n cleanup-env python=3.8
```

```sh
conda activate cleanup-env
```

Install packages:

```sh
pip install -r requirements.txt
```

Copy the default products inventory (then optionally customize the resulting "products.csv" file with your own products as desired):

```sh
cp data/default_products.csv data/products.csv
```




## Configuration

Obtain a premium AlphaVantage API Key [here](https://www.alphavantage.co/).

Sign up for a [SendGrid Account](https://sendgrid.com/), verify single sender, then obtain a Sendgrid API Key.


Set environment variables using a ".env" file approach:

```sh
ALPHAVANTAGE_API_KEY="..."

SENDER_ADDRESS="example@gmail.com"
SENDGRID_API_KEY="SG...."
```


## Usage

Run the game:

```sh
python app/game.py
```

Run the inventory report:

```sh
python -m app.groceries.py
```

Run the stocks report:

```sh
python -m app.stocks.py
```

Run the crypto report:

```sh
python -m app.crypto.py
```

## Testing

Running all tests:

```sh
pytest
```
