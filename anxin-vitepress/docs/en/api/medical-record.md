# Medical Record

## Create Medical Record

- **Endpoint**: `/api/medical-record`
- **Method**: `POST`
- **Request Type**: `application/x-www-form-urlencoded, application/json`
- **Response Type**: `*/*`

### Request Parameters

| Name                  | Description         | Required | Type   |
| --------------------- | ------------------ | -------- | ------ |
| patientId             | Patient ID         | No       | string |
| doctorId              | Doctor ID          | No       | string |
| departmentId          | Department ID      | No       | string |
| appointmentId         | Appointment ID     | No       | string |
| visitDate             | Visit Date         | No       | string |
| chiefComplaint        | Chief Complaint    | No       | string |
| presentIllness        | Present Illness    | No       | string |
| pastHistory           | Past History       | No       | string |
| physicalExamination   | Physical Exam      | No       | string |
| auxiliaryExamination  | Auxiliary Exam     | No       | string |
| diagnosis             | Diagnosis          | No       | string |
| treatmentPlan         | Treatment Plan     | No       | string |
| followUpPlan          | Follow-up Plan     | No       | string |

### Request Example

```json
{
  "patientId": "1",
  "doctorId": "2",
  "departmentId": "3",
  "appointmentId": "4",
  "visitDate": "2024-06-01",
  "chiefComplaint": "Headache",
  "presentIllness": "2 days",
  "pastHistory": "None",
  "physicalExamination": "Normal",
  "auxiliaryExamination": "CT normal",
  "diagnosis": "Cold",
  "treatmentPlan": "Drink more water",
  "followUpPlan": "Recheck in a week"
}
```

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": true
}
```

---

## Get Medical Record Details

- **Endpoint**: `/api/medical-record/{id}`
- **Method**: `GET`

### Path Parameters

| Name | Description   | Required | Type   |
| ---- | ------------- | -------- | ------ |
| id   | Medical ID    | Yes      | string |

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": {
    "id": "1",
    "patientId": "1",
    "doctorId": "2",
    "departmentId": "3",
    "appointmentId": "4",
    "visitDate": "2024-06-01",
    "chiefComplaint": "Headache",
    "presentIllness": "2 days",
    "pastHistory": "None",
    "physicalExamination": "Normal",
    "auxiliaryExamination": "CT normal",
    "diagnosis": "Cold",
    "treatmentPlan": "Drink more water",
    "followUpPlan": "Recheck in a week"
  }
}
``` 