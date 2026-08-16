# HOSxP Version 3.66.11.00

SQL scripts for extracting data from **HOSxP version 3.66.11.00** for educational and research purposes only.

**Non-commercial use only.**

These scripts can be used for exporting and reviewing patient-related data, OPD records, telemedicine information, drug allergy history, service costs, and other healthcare-related data.

> **Important:** This project does not include an ER Diagram or any existing database documentation.

---

## Available SQL Scripts

| Script                       | Description                                             |
| ---------------------------- | ------------------------------------------------------- |
| `check_daily_patient.sql`    | Check patients who received services on a specific date |
| `check_service_cost.sql`     | Check patient service costs and expenses                |
| `dtx_export.sql`             | Export DTX records                                      |
| `masked_patient.sql`         | Mask patient information according to PDPA principles   |
| `export_service_cost.sql`    | Export healthcare service cost information              |
| `migration_patient_data.sql` | Migrate patient data to Son Buddy                       |
| `telemedicine_export.sql`    | Export patients who received telemedicine services      |
| `view_allergy_history.sql`   | View patient drug allergy history                       |
| `view_village.sql`           | View village information                                |

---

## HOSxP Database Structure

### Treatment Rights and Basic Information

| Table        | Description                                |
| ------------ | ------------------------------------------ |
| `pttype`     | Patient healthcare entitlement information |
| `occupation` | Patient occupation information             |
| `religion`   | Patient religion information               |

### OPD (Outpatient Department)

| Table           | Description                                                                |
| --------------- | -------------------------------------------------------------------------- |
| `patient`       | General patient information                                                |
| `ovst`          | Patient visit information                                                  |
| `vn_stat`       | Visit and related service cost information                                 |
| `opdscreen`     | Patient screening information                                              |
| `ovstdiag`      | Diagnosis and treatment information                                        |
| `ptcardno`      | Patient national identification card information                           |
| `pttypeno`      | Healthcare entitlement number and related information                      |
| `occupation`    | Patient occupation information                                             |
| `pttype`        | Healthcare entitlement type                                                |
| `spclty`        | Medical department/specialty information                                   |
| `kskdepartment` | Service points, examination rooms, and healthcare units                    |
| `thaiaddress`   | Patient address information, including subdistrict, district, and province |

---

## Usage

1. Open the **SQL Editor** in HOSxP, usually accessible through the lightning-bolt icon, or use another database client that can connect to the HOSxP database.
2. Open the SQL script you want to run, for example:

   * `view_village.sql`
   * `view_allergy_history.sql`
   * `export_service_cost.sql`
3. Review the SQL query before execution.
4. Click **Run** to execute the script.
5. The query results can be exported to formats such as **CSV, Excel, or JSON**, depending on the database client being used.

> **Recommendation:** Use a **read-only database account** when running these scripts to reduce the risk of accidentally modifying production data.

---

## Data Privacy and Security

These scripts may access sensitive patient information.

Users are responsible for ensuring that any use, processing, storage, transfer, or disclosure of patient data complies with applicable laws, regulations, institutional policies, and data protection requirements.

For research or development purposes:

* Use anonymized or masked data whenever possible.
* Avoid exporting unnecessary personally identifiable information (PII).
* Do not expose patient data in public repositories.
* Do not commit real patient data, database dumps, or credentials to Git repositories.
* Use a read-only database account whenever possible.
* Test SQL scripts in a non-production environment before using them against a production database.

The `masked_patient.sql` script is provided as a data-masking example and should **not** be considered a complete guarantee of anonymization or regulatory compliance.

---

## Disclaimer

These SQL scripts are provided for **educational and research purposes only**.

The scripts are provided **"as is"**, without any warranty regarding accuracy, completeness, compatibility, performance, or suitability for a particular purpose.

Users should review and test every SQL query against their own HOSxP database environment before using it.

The database structure, table names, column names, relationships, and available fields may differ between HOSxP versions, configurations, or customized installations.

**Always create appropriate backups and verify queries before executing them on production systems.**

---

## Author

**Ratchanon Noknoy**

Computer Technical Officer

* GitHub: [ratchanon-noknoy2318](https://github.com/ratchanon-noknoy2318)
* LinkedIn: [linkedin.com/in/ratchanon-noknoy](https://www.linkedin.com/in/ratchanon-noknoy/?locale=th-TH)

---

## License and Usage

This project is intended for **non-commercial educational and research use only**.

Please review the repository license and applicable organizational policies before using, modifying, distributing, or integrating these scripts into other systems.
