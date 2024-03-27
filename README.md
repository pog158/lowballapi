# Minecraft Lowball API

This API calculates the lowball value for a Minecraft IGN based on certain parameters.

## Usage

To use this API, follow these steps:

1. **Send a GET Request**

   Send a GET request to the following endpoint to calculate the lowball value for a Minecraft IGN:

   ```
   GET https://lowballapi.ongfr.lol/lowball?username=<minecraft_ign>
   ```

   Replace `<minecraft_ign>` with the Minecraft in-game name (IGN) for which you want to calculate the lowball value.

   Example:

   ```
   GET https://lowballapi.ongfr.lol/lowball?username=example_username
   ```

2. **Response**

   The API will respond with a JSON object containing the username, lowball value, and breakdown of the calculation.

   Example Response:

   ```json
   {
     "username": "example_username",
     "lowball_value": 1000,
     "breakdown": {
       "skillAverage": 100,
       "catacombs": 200,
       "hotm": 150,
       "slayers": 30,
       "networth": 250
     }
   }
   ```

## Example

Here's an example of how to use the API using cURL:

```bash
curl -X GET "https://lowballapi.ongfr.lo/lowball?username=example_username"
```



## Contributing

Contributions are welcome! Feel free to open issues or pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
