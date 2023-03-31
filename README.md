
# Database Readme

## Schema

### Alerts Table
| Entry | Type | Notes |
| ------ | ---- | ----- |
| alert_id | INT | Primary Key, NOT NULL|
| employee_id | INT | NOT NULL |
| device_id | INT | NOT NULL |
| threshold | NUMERIC | NOT NULL |
| max | INT | NOT NULL |

### Devices Table
| Entry | Type | Notes |
| ----- | ---- | ----- |
| device_id | INT | Primary Key, NOT NULL |
| group_id | INT | |
| type | TEXT | |
| show | INT | NOT NULL, DEFAULT 1 |
| device_name | TEXT | NOT NULL |
| product_number | INT | NOT NULL |

### Employees Table
| Entry | Type | Notes |
| ----- | ---- | ----- |
| employee_id | INT | Primary Key, NOT NULL |
| username | TEXT | |
| password | TEXT | |
| email | TEXT | |
| first_name | TEXT | |
| last_name | TEXT | |

### Events Table
| Entry | Type | Notes |
| ----- | ---- | ----- |
| event_id | INT | Primary Key, NOT NULL |
| device_id | INT | |
| value | TEXT | |
| datetime | TEXT | | 
| event_type | TEXT | NOT NULL |

### Groups Table
| Entry | Type | Notes |
| ----- | ---- | ----- |
| group_id | INT | Primary Key, NOT NULL |
| group_name | TEXT | NOT NULL |

