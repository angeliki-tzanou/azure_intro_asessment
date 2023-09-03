{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "authorship_tag": "ABX9TyMynMCj+08fmzsrKbAgnl43",
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/angeliki-tzanou/azure_intro_asessment/blob/main/Copy_of_hha507class1.md\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "# Loading Packages"
      ],
      "metadata": {
        "id": "30Ie_qjkz4ad"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import pandas as pd\n",
        "import seaborn as sns\n",
        "import plotly as plt"
      ],
      "metadata": {
        "id": "znyIeccfzh0D"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "!pip freeze > packages.txt"
      ],
      "metadata": {
        "id": "tutsifNuzwWU"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "# Creating Functions"
      ],
      "metadata": {
        "id": "Q77f-KdpyoHR"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "def bloodpress(systolic, diastolic):\n",
        "  total = systolic + diastolic\n",
        "  return total"
      ],
      "metadata": {
        "id": "YyIqY9GHxPJP"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "def bloodsugar(value):\n",
        "  valuetoprint = f\"Your blood sugar is {value}\"\n",
        "  return valuetoprint"
      ],
      "metadata": {
        "id": "u7MeW3-vx-jb"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "# Testing Functions"
      ],
      "metadata": {
        "id": "puDBPlTmyd7u"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# Test for Blood Pressure\n",
        "\n",
        "test1 = bloodpress(190, 155)\n",
        "test1"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "MM9b8rLtyiI8",
        "outputId": "4e4a470b-b1c6-405b-d865-30554f46cebf"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "345"
            ]
          },
          "metadata": {},
          "execution_count": 5
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "test2 = bloodsugar(200)\n",
        "print(test2)"
      ],
      "metadata": {
        "id": "vyWLzersyqp2",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "866afae9-30f9-41ca-c8b9-b28abd88a5bd"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Your blood sugar is 200\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "test3 = bloodsugar(500)\n",
        "print(test3)"
      ],
      "metadata": {
        "id": "p33XwRlK3ZKy",
        "outputId": "8ce19ec2-f54f-4a11-adf6-34a41aeaa024",
        "colab": {
          "base_uri": "https://localhost:8080/"
        }
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Your blood sugar is 500\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(f\"\\n {test2} \\n {test3}\")"
      ],
      "metadata": {
        "id": "bU0cUe7i3jRE",
        "outputId": "9eabc0df-1c37-4791-8d09-41503265635e",
        "colab": {
          "base_uri": "https://localhost:8080/"
        }
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "\n",
            " Your blood sugar is 200 \n",
            " Your blood sugar is 500\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "# Pandas Data Loading Section"
      ],
      "metadata": {
        "id": "B_6PLEbv7KG1"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Example 1 with CSV files"
      ],
      "metadata": {
        "id": "-qrgOElh7qtL"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "stonybrook_east = pd.read_csv('https://raw.githubusercontent.com/hantswilliams/HHA_504_2023/main/WK1/data/113243405_StonyBrookEasternLongIslandHospital_standardcharges.csv')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 179
        },
        "id": "a1JtAq-278sQ",
        "outputId": "8251cdb2-49c8-49c9-da3a-2def3490ce87"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "error",
          "ename": "NameError",
          "evalue": "ignored",
          "traceback": [
            "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
            "\u001b[0;31mNameError\u001b[0m                                 Traceback (most recent call last)",
            "\u001b[0;32m<ipython-input-10-ae6de352880e>\u001b[0m in \u001b[0;36m<cell line: 1>\u001b[0;34m()\u001b[0m\n\u001b[0;32m----> 1\u001b[0;31m \u001b[0mstonybrook_east\u001b[0m \u001b[0;34m=\u001b[0m \u001b[0mpd\u001b[0m\u001b[0;34m.\u001b[0m\u001b[0mread_csv\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;34m'https://raw.githubusercontent.com/hantswilliams/HHA_504_2023/main/WK1/data/113243405_StonyBrookEasternLongIslandHospital_standardcharges.csv'\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n\u001b[0m",
            "\u001b[0;31mNameError\u001b[0m: name 'pd' is not defined"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Example 2 of loading CSV"
      ],
      "metadata": {
        "id": "jYMAP-kK9VRd"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "dataset2 = pd.read_csv('')"
      ],
      "metadata": {
        "id": "HZex9gaE9Y9g"
      },
      "execution_count": null,
      "outputs": []
    }
  ]
}