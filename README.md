# Xmrit

Xmrit is the easiest tool to work with the [XmR process-control chart](https://xmrit.com/about/). It is a simple web-based application that allows you to create a chart by pasting in data, interacting with the chart, and sharing it.

A live version of the tool is available at http://xmrit.com/t/ . You can find more details on the tool by reading the [user manual](https://xmrit.com/manual/) or the [integration guide](https://xmrit.com/integration/). All data is stored in your browser and will never be shared with anyone (including us!) as per our [privacy policy](https://xmrit.com/privacy/).

## Getting Started

1. [Download the latest release](https://github.com/xmrit/xmrit/releases).
2. Start a local http server from the directory
  - We assume you have python installed
    ```
    python -m http.server 5000
    ```
3. Now, open your browser at http://localhost:5000 and voila! You're ready to go.

## Contributing

### Development setup

The following steps will get you set up to contribute changes to this repo:

1. Fork the repo (Click the Fork button at the top of [this page](https://github.com/xmrit/xmrit))
2. Clone your fork locally
3. Install dependencies by running `npm install`
4. Start local dev server by running `npm run start`

## Notebooks: XmR charts for business metrics

A self-contained Google Colab notebook that teaches, with synthetic data and known injected signals, how to apply XmR charts to weekly business-review metrics: day-of-week and annual seasonality, new locations with no baseline, sustained growth, limit recalculation and phase charts, and a set of common pain points (variable denominators, rare events, bounded metrics, lagged outcomes, mix shift, roll-up masking, calendar artifacts, targets vs. natural limits). It ends with an executive translation layer and a metric-registry pattern for productising the approach.

It comes in two versions with identical content:

| Version | Use it to | Open |
|---|---|---|
| `notebooks/xmr_business_metrics_colab.ipynb` | run the code yourself (outputs cleared) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HarrisonGrubb/xmrit/blob/main/notebooks/xmr_business_metrics_colab.ipynb) |
| `notebooks/xmr_business_metrics_colab_executed.ipynb` | read it with every chart and result already rendered | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HarrisonGrubb/xmrit/blob/main/notebooks/xmr_business_metrics_colab_executed.ipynb) |

Both produce the same results because all data comes from a fixed random seed. You can also open either one in Colab with `File → Open notebook → GitHub` and the file path.
