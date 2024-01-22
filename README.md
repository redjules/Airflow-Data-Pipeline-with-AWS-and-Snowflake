# Airflow-Data-Pipeline-with-AWS-and-Snowflake

We will use Python SDK:
<img width="648" alt="Screenshot 2024-01-22 at 10 28 25" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/973d8da7-818f-4e62-9f11-81768a66fbfa">



Goal:

<img width="674" alt="Screenshot 2024-01-22 at 09 25 38" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/f9715755-23b9-40b3-964a-a0390a1c0796">


Prerequisites:

<img width="683" alt="Screenshot 2024-01-22 at 09 19 11" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/ec6a1a9a-212c-48a3-bb9d-39161949a26c">

Install Astro CLI:


<img width="538" alt="Screenshot 2024-01-22 at 10 27 18" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/6481408a-c70a-4146-9152-a3162b021349">


Initialize astro:

<img width="415" alt="Screenshot 2024-01-22 at 10 27 42" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/abfd331e-d5f4-41bb-86ef-e51ec7ef7be2">


update env and requirements:
<img width="581" alt="Screenshot 2024-01-22 at 10 28 55" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/41814811-e64e-456d-aebe-f7ae339ea867">

<img width="615" alt="Screenshot 2024-01-22 at 10 29 09" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/338a2a9d-86e4-4089-b7b9-ee9c773575aa">


in Terminal: astro dev start
<img width="406" alt="Screenshot 2024-01-22 at 10 29 27" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/7667e85f-ad22-4433-a1ba-8f872e8ff17f">

Go to localhost 8080 and access Airflow
<img width="795" alt="Screenshot 2024-01-22 at 10 29 43" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/9070c124-78b7-470f-993e-c83b2ce50690">

Create orders in data Folder:

<img width="742" alt="Screenshot 2024-01-22 at 10 30 23" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/caec250f-bb21-4ab2-891b-70bae22444d9">

Create s3 in AWS:
<img width="660" alt="Screenshot 2024-01-22 at 10 32 38" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/e35fb0b5-609a-487f-9c3d-3a3e1201a974">

We create an AWS IAM user:

<img width="586" alt="Screenshot 2024-01-22 at 10 42 14" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/70d46131-ec19-44ec-9a94-2e5f15c63428">

Go to Snowflake and create a Worksheet and a database:

<img width="540" alt="Screenshot 2024-01-22 at 10 45 44" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/56221a5e-4e86-4b03-8bda-15987f1e5e19">

Create a Warehouse, Schema and a Table:

<img width="230" alt="Screenshot 2024-01-22 at 10 46 31" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/28a82c6c-485f-40c2-bbe1-11480896f451">

<img width="586" alt="Screenshot 2024-01-22 at 10 46 52" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/94296fa6-1f6e-48fc-81a9-59bac0fa4a9d">

<img width="732" alt="Screenshot 2024-01-22 at 10 47 10" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/96c06bdb-f9c8-4258-84d0-7256b88005c8">

<img width="689" alt="Screenshot 2024-01-22 at 10 47 36" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/230706be-5191-47bb-a0ce-0c6abb6a1bbb">

<img width="524" alt="Screenshot 2024-01-22 at 10 47 45" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/78ea5657-548a-4c5d-b955-5a51be44e2a4">

We create the connections in Airflow:

<img width="762" alt="Screenshot 2024-01-22 at 10 48 46" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/1597bace-35df-4df1-b4c1-7cb173099623">

<img width="641" alt="Screenshot 2024-01-22 at 10 49 10" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/0db77aed-ec8e-4a37-8dde-839473c8cb48">

<img width="573" alt="Screenshot 2024-01-22 at 10 50 39" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/2c3ed9e5-6106-48e3-91a8-9cc94ebd159d">

Now go to VSCode and create astro_orders.py:

<img width="917" alt="Screenshot 2024-01-22 at 11 05 05" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/c0569196-d753-4a09-8ce2-7daa1fe31a86">
<img width="694" alt="Screenshot 2024-01-22 at 11 05 20" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/847b9632-ab7b-4bac-8bf4-0d589e1cd51a">

we add the decorators aql.transform:
<img width="596" alt="Screenshot 2024-01-22 at 11 07 04" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/b507200e-eabe-48a1-b084-abda7c4302cf">

<img width="754" alt="Screenshot 2024-01-22 at 11 07 36" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/47aed020-a8d1-46d8-a171-9ecce08da04f">

we do a join between the joined data and the reporting table:
<img width="744" alt="Screenshot 2024-01-22 at 11 08 35" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/7c96420b-6fb9-4927-b3fa-5eab681dd3ed">
<img width="589" alt="Screenshot 2024-01-22 at 11 09 17" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/d2d67e64-779a-41df-8d5b-0a50ae4f373f">

we convert sql table into database:
<img width="631" alt="Screenshot 2024-01-22 at 11 10 54" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/a6b2bd34-b836-4d7f-98a2-a5308d17cb04">

we clean up the temporary tables that we have created when  we use tbale without specifying the name:
<img width="778" alt="Screenshot 2024-01-22 at 11 11 38" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/777970a9-5fe1-4924-836c-9be4d1a247e1">


Final result:

<img width="703" alt="Screenshot 2024-01-22 at 11 14 15" src="https://github.com/redjules/Airflow-Data-Pipeline-with-AWS-and-Snowflake/assets/106017493/03e84150-70c1-43a8-8e1f-abc9cabb5a19">

First you will load the file that was uploaded in S3 into the table, you'll filer the orders from that table and you will join the orders with the customers. You will merge the data into the reporting table to finally transform the data from the reporting table to get the purchase dates and finally ypu will clean all the temporary tables that were created along the way.
