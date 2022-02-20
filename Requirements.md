# Requirements

1. Main
- 1-1. An application which has version control.
- 1-2. The statemachine shall have Init, Idle, Progress, Alarm, Deinit.
- 1-3. Support multi-threads execution since each Cmd shall be independent to each others.
2. Logger
- 2-1. Apply queue memory to store the LogMsg.
- 2-2. Write LogMsg into specificed file.
- 2-3. Periodically write into file.
3. IniHandler: Read file setting to avoid hard coding
- 3-1. Read setting from ini file.
- 3-2. Write setting into ini file.
4. Scrapter: Connect to Website and query raw data
- 4-1. Connect to Website.
- 4-2. Get whole html info or scrapt whole data.
- 4-3. Check scrapt success or not.
- 4-4. Time-out mechanism is required.
- 4-5. Error handling is required.
5. DBHandler: Export file
- 5-1. Connect to Database.
- 5-2. Read data from Database.
- 5-3. Write data into Database.
- 5-4. Time-out mechanism is required.
- 5-5. Error handling is required.
6. Parser: Refine raw data (The adapter between Scrapter & DB)
- 6-1. Parse data from raw data.
- 6-2. Generate refined data for DB export.
- 6-3. Error handling is required.
