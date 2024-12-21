--Total Charge Amount per provider by department
select
  concat(p.firstname, ' ', p.LastName) Provider_Name,
  dd.Name Dept_Name,
  sum(ft.Amount)
from
  gold.fact_transactions ft
  left join gold.dim_provider p on p.ProviderID = ft.FK_ProviderID
  left join gold.dim_department dd on dd.Dept_Id = p.DeptID
group by
  all 
  
  
--Total Charge Amount per provider by department for each month for year 2024
select
  concat(p.firstname, ' ', p.LastName) Provider_Name,
  dd.Name Dept_Name,
  date_format(servicedate, 'yyyyMM') YYYYMM,
  sum(ft.Amount) Total_Charge_Amt,
  sum(ft.paidamount) Total_Paid_Amt
from
  gold.fact_transactions ft
  left join gold.dim_provider p on p.ProviderID = ft.FK_ProviderID
  left join gold.dim_department dd on dd.Dept_Id = p.DeptID
where
  year(ft.ServiceDate) = 2024
group by
  all
order by
  1,
  3
