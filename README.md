## Myanmar Currency API Documentation

### Introduction
The Myanmar Currency API provides real-time exchange rate data for various currencies against the Myanmar Kyat (MMK). This API is suitable for developers who need accurate and up-to-date currency exchange information for their applications.

### Accessing the API
The API can be accessed through a simple HTTP GET request to the following endpoint:
```
https://myanmar-currency-api.github.io/api/latest.json
```

### Response Format
The API response is in JSON format and contains the following fields:

- `data`: An array of objects, each representing a currency exchange rate. Each object has the following attributes:
  - `currency`: The currency code (e.g., USD, EUR, SGD).
  - `buy`: The buying rate of the currency against Myanmar Kyat.
  - `sell`: The selling rate of the currency against Myanmar Kyat.
- `epoch`: UNIX timestamp indicating the time when the data was last updated.
- `timestamp`: Human-readable date and time of the last update in the format "YYYY-MM-DD HH:MM:SS".

### Example Response
```json
{
    "data": [
        {
            "currency": "USD",
            "buy": "3500",
            "sell": "3450"
        },
        {
            "currency": "EUR",
            "buy": "3807",
            "sell": "3730"
        },
        {
            "currency": "SGD",
            "buy": "2595",
            "sell": "2545"
        },
        {
            "currency": "MYR",
            "buy": "749",
            "sell": "734"
        },
        {
            "currency": "CNY",
            "buy": "490.00",
            "sell": "480.00"
        },
        {
            "currency": "THB",
            "buy": "99.00",
            "sell": "97.00"
        },
        {
            "currency": "JPN",
            "buy": "23.79",
            "sell": "23.31"
        }
    ],
    "epoch": 1707491029.7016091,
    "timestamp": "2024-02-09 21:33:49"
}
```

### Data Source
The exchange rate data provided in this API is sourced from reputable financial markets and is periodically updated. Additionally, news updates and market analysis from the DVB TV News YouTube channel are considered as supplementary sources to ensure accuracy and relevance.

### Rate Limits
Currently, there are no rate limits imposed on API requests. However, please use the API responsibly and avoid excessive polling to prevent unnecessary load on the server.

### Data Accuracy and Ambiguity
While we strive to provide accurate and up-to-date exchange rate data, occasional discrepancies or ambiguities may arise due to rapid market fluctuations or data processing issues. In such cases, we encourage users to cross-reference information with trusted sources, including the DVB TV News YouTube channel, for clarification and verification.

### Support and Feedback
For any questions, issues, or feedback regarding the Myanmar Currency API, please open an issue on the GitHub repository: [Myanmar Currency API GitHub Repository](https://github.com/myanmar-currency-api).

### Terms of Use
By using the Myanmar Currency API, you agree to abide by the terms of use outlined in the LICENSE file available in the repository.
