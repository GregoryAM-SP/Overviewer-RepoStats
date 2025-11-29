### The Minecraft Overviewer Data (RepoStatistics)

The following data is used on [The Minecraft Overviewer Website](https://overviewer.gregoryam.com).

The GitHub Action uses GitHub API to pull the data from [The Minecraft Overviewer repository](https://github.com/gregoryam-sp/the-minecraft-overviewer) to update data on the website.

Which includes the following:

- The Release Tags
- The Release Assets
- The Release Asset URLs
- The Total Downloads for each Release
- The Total Amount of Forks for the Repository
- The Total Amount of Stars / Watchers for the Repository

Since I am unsure when the next release will be, I run a CRON job every 6 hours to update the data. This will continue indefinitely.

I also check the Rate Limit on every Action to make sure we are not going to hit the Rate Limit. Which you can check [here](https://github.com/GregoryAM-SP/Overviewer-RepoStats/actions)

<hr>

You may review the data in the [data.json](https://github.com/GregoryAM-SP/Overviewer-RepoStats/blob/main/data.json) file.

You may also view the GitHub Action workflow in the [generate_json.yml](https://github.com/GregoryAM-SP/Overviewer-RepoStats/blob/main/.github/workflows/generate_json.yml) file to understand how the data is retrieved.

I use Python to retrieve the data from the GitHub API.

<hr>

