# medical-waste-treatment-system-by-ARAS_H_IW
The ARAS_H_IW medical waste treatment system is a Python web application that integrates the entire pipeline of the ARAS-H-IW approach (based on the ARAS method: Additive Ratio Assessment which is extended to a hesitant fuzzy environment and integrating an inverse inference mechanism of the weights of the IW criteria).
====================================================
Steps to deploy the application:

1) Download the folder to Windows
2) Go to the project folder: right-click on it and select "Open in Terminal"

Result: PS C:\my_project
3) Then, in the terminal, run the following command to activate the virtual environment:
.\.venv\Scripts\Activate.ps1

You should see (.venv) at the beginning of the line.

4) Install/update dependencies (once, or after modification)
`python -m pip install --upgrade pip`
`python -m pip install -r requirements.txt`
`python -m pip install -U python-docx`

5) Launch the Streamlit application
`python -m streamlit run app.py`

6) Then open:

http://localhost:8501

If you want network (LAN) access
`python -m streamlit run app.py --server.address 0.0.0.0 --server.port 8501`

If you want to enable login (optional)

Before launching:

`$env:APP_USERNAME="admin"`
`$env:APP_PASSWORD="StrongPass123!"`
`python -m streamlit run app.py`
