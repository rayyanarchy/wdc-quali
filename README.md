# F1 WDC Contenders

A Formula 1 web app that determines which drivers are still mathematically in contention for the World Drivers' Championship. The project uses current championship standings and the maximum points available in the remaining races to identify drivers who can still catch the championship leader.

> This project is not affiliated with, endorsed by, or associated with Formula 1, the FIA, or any Formula 1 teams.

## How It Works

For each driver, the app:

1. Fetches the current F1 driver standings.
2. Determines the remaining races and their available points, including Sprint weekends.
3. Calculates each driver's maximum possible season total.
4. Compares that total with the current championship leader.
5. Marks each driver as either **IN FIGHT** or **OUT**.

The current version uses a deterministic mathematical calculation. A **Jev-based probability model** is planned to estimate each driver's probability of becoming the eventual WDC.


## Tech Stack

* **Python**
* **Flask** — web application
* **FastF1** — F1 data and event schedules
* **Pandas** — data processing
* **Jev** — planned probabilistic modelling


## Roadmap

* [ ] Add Jev-based WDC probability model
* [ ] Improve the web UI
* [ ] Investigate support for historical seasons
* [ ] Evaluate migration from Render to Vercel for improved deployment performance


## License

This project is open source and available under the [MIT License](LICENSE).
