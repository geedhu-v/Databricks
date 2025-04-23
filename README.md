# Databricks

## Structured Streaming
<br> Readstream Syntax <br>
<img width="914" alt="image" src="https://github.com/user-attachments/assets/709f705d-0714-4b38-b93d-da6258938fef" />
<br> Writestream Syntax <br>
<img width="909" alt="image" src="https://github.com/user-attachments/assets/3e0ec317-a9ed-478e-9ac0-f74bf4f765f3" />

#### Trigger levels
<br>1. Unspecified - defauly processing time = 500ms
<br>2. Fixed Intervals - .trigger(processingTime = "5 minutes")
<br>3. Triggered batch - .trigger(once = True)
<br>4. Triggerred micro batch - .trigger(availableNow = True)

#### Output Mode
<br> 1. Append (default mode)
<br> 2. Complete - preferred for aggregate operations as result set table will be re-calculated for every write stream trigger.

