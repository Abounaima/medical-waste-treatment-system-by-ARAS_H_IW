# medical-waste-treatment-system-by-ARAS_H_IW
The ARAS-H-IW decision support system for medical waste management is a web application developed in Python that integrates the entire proposed methodological pipeline. It is based on the Additive Ratio Assessment (ARAS) method, extended to a hesitant fuzzy environment to explicitly represent expert hesitation and data uncertainty, while incorporating an inverse weighting inference mechanism to estimate criterion weights based on decision preferences rather than imposing them a priori. The tool aims to support optimal and rational selection of medical waste treatment technologies in Morocco, with a focus on the Fes-Meknes region, where the decision simultaneously depends on economic, environmental (emissions and energy), health, regulatory (compliance/traceability), and socio-organizational (HSE risks, acceptability, flexibility) dimensions.
====================================================
Steps to deploy the application:

1) Download the folder to Windows
2) Go to the project folder: right-click on it and select "Open in Terminal"

Result: PS C:\my_project

3) Then, in the terminal, run the following commands to activate the virtual environment:
     i) python -m venv .venv
   ii) .\.venv\Scripts\Activate.ps1
You should see (.venv) at the beginning of the line.

4) Install/update dependencies (once, or after modification)
i) `python -m pip install --upgrade pip`
ii) `python -m pip install -r requirements.txt`
iii) `python -m pip install -U python-docx`

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
