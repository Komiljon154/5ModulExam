# 📝 ToDoList Project

Bu loyiha `ToDo List` ilovasining backend qismini yaratadi. Loyihada **SQL Server**, **ADO.NET**, **FluentValidation**, **AutoMapper**, va **Layered Architecture** (qatlamli arxitektura) qo‘llanilgan. Maqsad – CRUD amallarini bajarish va vazifalarni boshqarish uchun mustahkam RESTful API yaratish.

---

## 📦 Texnologiyalar

- **Backend**: .NET Core Web API  
- **Database**: Microsoft SQL Server  
- **ORM**: ADO.NET  
- **Validation**: FluentValidation  
- **Mapping**: AutoMapper  
- **Architecture**: Layered Architecture (API, BLL, DAL, Models)  
- **Version Control**: Git + GitHub  

---

## 📁 Layerlar

- **API Layer**: Controller va endpointlar joylashgan.  
- **BLL (Business Logic Layer)**: Biznes mantiq joylashgan.  
- **DAL (Data Access Layer)**: SQL bilan ishlovchi kodlar joylashgan. `Queries.sql` fayli orqali barcha `CREATE TABLE` va `Stored Procedure` lar saqlangan.  
- **Models**: Entity/model klasslar.

---

## 🧩 Model

```csharp
public class ToDoItem
{
    public long ToDoItemId { get; set; }
    public string Title { get; set; }
    public string Description { get; set; }
    public bool IsCompleted { get; set; }
    public DateTime CreatedAt { get; set; }
    public DateTime DueDate { get; set; }
}
