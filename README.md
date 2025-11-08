Objective

The goal of this project is to develop a predictive model that estimates the likelihood of rear axle crown wheel–pinion failure in commercial vehicles based on design, operational, and environmental parameters.
The analysis aims to identify key factors influencing failure and guide design improvements, maintenance schedules, and operational best practices to enhance axle reliability.

🧩 Dataset Overview

The dataset consists of 3,000 total records, representing two classes:

1,200 failed (Failure = 1) cases

1,800 non-failed (Failure = 0) cases

Each record describes the rear axle system condition, grouped into three categories:

1️⃣ Design Parameters

Define the geometry, material, and stiffness of the gearset and axle housing.
Key variables include:

Module_mm, Face_Width_mm, Pressure_Angle_deg, Contact_Ratio, Backlash_mm

Case_Depth_mm, Surface_Hardness_HRC, Runout_mm, Housing_Stiffness_index, Material_Grade

Torque_Speed_Ratio, Thermal_Stress_Index, Aging_Factor

2️⃣ Operational Parameters

Represent vehicle usage, load conditions, lubrication, and maintenance.
Key variables include:

Load_Torque(Nm), Speed(RPM), Vehicle_Load(kg), Lubricant_Temp(°C), Oil_Viscosity(cSt)

Maintenance_Gap(km), Brake_Usage_Freq(/100km), Lubrication_Efficiency, Oil_Contamination_Index

Noise_Level(dB), Vibration(mm/s), Shock_Severity_Index, Temperature_Rise(°C), Cumulative_Damage_Index

3️⃣ Environmental Parameters

Capture the operating environment’s effect on axle performance.
Key variables include:

Ambient_Temp(°C), Humidity(%), Altitude(m), Road_Roughness(m/s²)

Road_Type, Dust_Level, Rain_Exposure

⚙️ Data Generation

The dataset is synthetically generated using controlled distributions to ensure realistic patterns:

Higher torque, load, temperature, vibration, and poor lubrication are more common in failed cases.

Optimal geometry, hardness, lubrication efficiency, and stiffness are dominant in non-failed cases.

Categorical variables like Road_Type, Shock_Load, Dust_Level, and Material_Grade follow logical distributions—e.g., High Dust and Low Material Grade are more likely in failure cases.
