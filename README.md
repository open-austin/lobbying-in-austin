# lobbying-in-Austin

Visualization of Austin lobbyist registrations.

Our plan is to take [lobbyist registration data from data.austintexas.gov](https://data.austintexas.gov/dataset/Lobbyists/bqav-9x6a), convert it to show lobbying activity by various organizations on different dates, and make a visualization in D3.js.

There are probably still significant errors in our modified versions of the dataset. If you need accuracy, please get your data directly from data.austintexas.gov for now.

## Datasets

* lobbyistFromCity.csv: This is closest to the dataset provided by data.austintexas.gov
* lobbyistDedupe.csv: An intermediate step created by running [csvdedupe](https://github.com/datamade/csvdedupe) to sort the previous dataset into clusters. Useful mainly for replicating our data cleaning process (see lobbyistsDedupe.ipynb).
* lobbyistTimeRange.csv: A list of time ranges when each lobbyist was employed by every client in the dataset.
* lobbyistByClient.csv: A list of how many lobbyists each client employed on every date (but without the lobbyists' names).
