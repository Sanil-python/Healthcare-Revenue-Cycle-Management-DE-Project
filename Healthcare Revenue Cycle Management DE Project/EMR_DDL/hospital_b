-- For database trendytech-hospital-b:

-- 2. Departments Table:

CREATE TABLE dbo.departments (
    DeptID nvarchar(50) NOT NULL,
    Name nvarchar(50) NOT NULL,
    CONSTRAINT PK_departments PRIMARY KEY (DeptID)
);

-- 2. Encounters Table:

CREATE TABLE dbo.encounters (
    EncounterID nvarchar(50) NOT NULL,
    PatientID nvarchar(50) NOT NULL,
    EncounterDate date NOT NULL,
    EncounterType nvarchar(50) NOT NULL,
    ProviderID nvarchar(50) NOT NULL,
    DepartmentID nvarchar(50) NOT NULL,
    ProcedureCode int NOT NULL,
    InsertedDate date NOT NULL,
    ModifiedDate date NOT NULL,
    CONSTRAINT PK_encounters PRIMARY KEY (EncounterID)
);

-- 3. Hospital2_Patient_Data Table:

CREATE TABLE dbo.patients (
    ID nvarchar(50) NOT NULL,
    F_Name nvarchar(50) NOT NULL,
    L_Name nvarchar(50) NOT NULL,
    M_Name nvarchar(50) NOT NULL,
    SSN nvarchar(50) NOT NULL,
    PhoneNumber nvarchar(50) NOT NULL,
    Gender nvarchar(50) NOT NULL,
    DOB date NOT NULL,
    Address nvarchar(100) NOT NULL,
    Updated_Date date NOT NULL,
    CONSTRAINT PK_patients PRIMARY KEY (ID)
);


-- 4. Providers Table:

CREATE TABLE dbo.providers (
    ProviderID nvarchar(50) NOT NULL,
    FirstName nvarchar(50) NOT NULL,
    LastName nvarchar(50) NOT NULL,
    Specialization nvarchar(50) NOT NULL,
    DeptID nvarchar(50) NOT NULL,
    NPI bigint NOT NULL,
    CONSTRAINT PK_providers PRIMARY KEY (ProviderID)
);


-- 5. Transactions Table:

CREATE TABLE dbo.transactions (
    TransactionID nvarchar(50) NOT NULL,
    EncounterID nvarchar(50) NOT NULL,
    PatientID nvarchar(50) NOT NULL,
    ProviderID nvarchar(50) NOT NULL,
    DeptID nvarchar(50) NOT NULL,
    VisitDate date NOT NULL,
    ServiceDate date NOT NULL,
    PaidDate date NOT NULL,
    VisitType nvarchar(50) NOT NULL,
    Amount float NOT NULL,
    AmountType nvarchar(50) NOT NULL,
    PaidAmount float NOT NULL,
    ClaimID nvarchar(50) NOT NULL,
    PayorID nvarchar(50) NOT NULL,
    ProcedureCode int NOT NULL,
    ICDCode nvarchar(50) NOT NULL,
    LineOfBusiness nvarchar(50) NOT NULL,
    MedicaidID nvarchar(50) NOT NULL,
    MedicareID nvarchar(50) NOT NULL,
    InsertDate date NOT NULL,
    ModifiedDate date NOT NULL,
    CONSTRAINT PK_transactions PRIMARY KEY (TransactionID)
);
