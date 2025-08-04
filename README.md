NCR Management – Power Platform řešení
Model‑driven aplikace pro evidenci Non‑Conformity Reports, nápravných opatření a příloh – připravená k nasazení do prostředí Microsoft Dataverse.

Funkce:
Non Conformity – formulář se statusem, typem, automatickým číslem NCR a vazbou na reportující osobu.

Corrective Actions – tabulka podřízených opatření.

Evidence – knihovna souborů svázaná s NCR číslem.

Rychlý start (lokální)

# 1 ) přihlášení k prostředí
pac auth create --url https://<org>.crm4.dynamics.com

# 2 ) rozbalení řešení (pokud jste stáhli jen ZIP)
pac solution unpack --zipfile NCR_1_0_0_1_managed.zip --folder src --packagetype Managed --clobber

# 3 ) import do prostředí
pac solution import --path NCR_1_0_0_1_managed.zip --publish-all --activate-plugins true

Požadavky:

Node JS ≥ 16 a npm

Power Platform CLI (pac)

Oprávnění Power Platform Administrator nebo sys‑admin v cílovém prostředí
