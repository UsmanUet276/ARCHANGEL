
> #### ⚠️⚠️ PLEASE BE AWARE THAT ARCHANGEL IS STILL IN ITS EARLY STAGES OF DEVELOPMENT AND MAY CONTAIN A LOT OF FALSE POSITIVES IN PREDICTION. THIS PROJECT IS DEVELOPED FOR EDUCATIONAL PURPOSES ONLY AND WE MAKE NO GUARANTEE THAT THE OUTPUT PRODUCED BY ARCHANGEL IS ABSOLUTELY CORRECT. SO PLEASE DO NOT JUDGE OTHER APPLICATIONS USING THE OUTPUT OF ARCHANGEL ALONE.⚠️⚠️
## About
ARCHANGEL is an attempt to detect malwares on android devices by utilizing machine learning approach.

## Features

- Real time scanning
- On device inference
- Lightweight
- 100% free and no ads

## How it works?

ARCHANGEL uses permissions and intent-filters to detect malicious apps. While scanning, it loads the machine learning model and extracts permissions and intents from the installed applications on the user's device. These extracted features are then fed to the machine learning model in the form of a vector. The machine learning model returns a prediction score between 0 and 1 that denote the degree of maliciousness of the scanned application. We use this score to classify the scanned app into one of the following categories:
1. Goodware: The prediction score is less than 0.5
2. Risky: Prediction score between 0.5 and 0.75
3. Malware: Prediction score is greater than 0.75
4. Unknown: If ARCHANGEL is unable to extract permissions and intents from an app, then that app is labelled as 'Unknown'

You can check the code for building machine learning model [here](https://github.com/projectmatris/antimalwareapp_ml)

## Open Source License

Unless explicitly stated otherwise all files in this repository are licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0-standalone.html).

    ARCHANGEL - Anti-malware for Android using machine learning
    Copyright (C) 2020 Project Matris

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <https://www.gnu.org/licenses/>.

An unmodified copy of the above license text must be included in all forks. 

> Android is a trademark of Google LLC.

