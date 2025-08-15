# pyXLMS-app

Permalink to the web application for [pyXLMS](https://github.com/hgb-bin-proteomics/pyXLMS).

- For the source code of the web application please refer to [pyXLMS/gui](https://github.com/hgb-bin-proteomics/pyXLMS/tree/master/gui).
- The web application is currently hosted at [http://pyxlms.projekte.fh-hagenberg.at/](http://pyxlms.projekte.fh-hagenberg.at/).
- A backup server is running at [http://89.58.32.151/](http://89.58.32.151/).
  - _Main server and backup server might not run the same pyXLMS version._

## Availability

Both the main and backup server are provided as is and availability is not guaranteed! Computing resources are allocated on a first come, first served basis.
Please note that no data is saved and any analysis only persists as long as your session is active in your browser!

## Running Locally or Self-Hosting

Additionally, the web application can also be run locally or self-hosted. **This is the preferred way if you are analyzing large amounts of data or**
**sensitive data.** You can run the web app locally or self-hosted via:

- Cloning the [pyXLMS GitHub repository](https://github.com/hgb-bin-proteomics/pyXLMS):
  - `git clone https://github.com/hgb-bin-proteomics/pyXLMS.git`
  - `cd pyXLMS`
- Running the [streamlit](https://streamlit.io/) app locally:
  - `cd gui`
  - `pip install -r requirements.txt`
  - `streamlit run streamlit_app.py`
- _or_ running via [Docker](https://docs.docker.com/get-started/get-docker/) by building the image yourself:
  - `docker build . -f Dockerfile -t pyxlms`
  - `docker run -p 8501:8501 pyxlms`
- _or_ by pulling the provided image from Docker Hub:
  - `docker run -p 8501:8501 michabirklbauer/pyxlms:latest`

## Contact

- [proteomics@fh-hagenberg.at](mailto:proteomics@fh-hagenberg.at)
- [micha.birklbauer@fh-hagenberg.at](mailto:micha.birklbauer@fh-hagenberg.at) (primary developer)
