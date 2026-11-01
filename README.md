[English version below](#english)

# Course Schedule

Öğretim elemanı, derslik, ders, bölüm ve fakülte yönetimi ile ders programı oluşturmayı sağlayan Windows Forms uygulaması.

## Özellikler

- Rol tabanlı giriş ekranı
- Fakülte, bölüm, öğretim elemanı, ders, grup ve derslik yönetimi
- Otomatik ders dağıtımı
- Takvim üzerinden manuel ders atama ve silme
- Öğretim elemanı çakışması ve sınıf kapasitesi gibi kısıt kontrolleri
- SQL Server üzerinde kalıcı veri yönetimi

## Teknolojiler

- C# / .NET 10
- Windows Forms
- Microsoft SQL Server
- `Microsoft.Data.SqlClient`
- MetroModernUI

## Proje Yapısı

- `CourseSchedule(Kaynak Kodları)/`: Uygulamanın kaynak kodu ve çözüm dosyası
- `CourseSchedule_DB.sql`: Veritabanı kurulum scripti
- `CourseScheduleErDiyagramı.png`: ER diyagramı
- `GPFinalRaporTaslagi.pdf` ve `CourseScheduleGereksinimAnalizi.pdf`: Teslim/analiz dokümanları

## Kurulum

1. SQL Server'ı yerelde çalıştırın.
2. `CourseSchedule_DB.sql` dosyasını SQL Server Management Studio'da çalıştırın.
3. Bağlantı ayarını gerekirse `CourseSchedule(Kaynak Kodları)/DatabaseHelper.cs` içinde kendi SQL Server örneğinize göre güncelleyin.
4. `CourseSchedule(Kaynak Kodları)/CourseSchedule.slnx` dosyasını Visual Studio ile açın ve derleyin; ya da proje klasöründe `dotnet build` çalıştırın.

## Gereksinimler

- .NET 10 SDK ve Windows
- SQL Server / SQL Server Express
- Visual Studio 2022 veya daha yeni bir sürüm (önerilir)

## Durum

Kaynak kodu .NET 10 ile başarıyla derlenmektedir. `MetroModernUI` paketinin modern .NET hedefi için uyumluluk uyarısı vermesi mümkündür.

## Ekip

Eyüp Karakaya ve Kağan Kemal Üre

-------------------------------------

## English

# Course Schedule

A Windows Forms application for managing instructors, classrooms, courses, departments and faculties, and for generating course schedules.

## Features

- Role-based login screen (Admin / Student view)
- Management of faculties, departments, instructors, courses, groups and classrooms
- Automatic course distribution
- Manual course assignment and removal directly on the calendar
- Constraint checks such as instructor conflicts and classroom capacity
- Persistent data storage on SQL Server

## Technologies

- C# / .NET 10
- Windows Forms
- Microsoft SQL Server
- `Microsoft.Data.SqlClient`
- MetroModernUI

## Project Structure

- `CourseSchedule(Kaynak Kodları)/`: Application source code and solution file
- `CourseSchedule_DB.sql`: Database setup script
- `CourseScheduleErDiyagramı.png`: ER diagram
- `GPFinalRaporTaslagi.pdf` and `CourseScheduleGereksinimAnalizi.pdf`: Final report draft and requirements analysis (in Turkish)

## Setup

1. Run SQL Server locally.
2. Run `CourseSchedule_DB.sql` in SQL Server Management Studio.
3. If needed, update the connection string in `CourseSchedule(Kaynak Kodları)/DatabaseHelper.cs` to match your SQL Server instance.
4. Open `CourseSchedule(Kaynak Kodları)/CourseSchedule.slnx` in Visual Studio and build it, or run `dotnet build` in the project folder.

## Requirements

- .NET 10 SDK and Windows
- SQL Server / SQL Server Express
- Visual Studio 2022 or later (recommended)

## Status

The source code builds successfully with .NET 10. The `MetroModernUI` package may show a compatibility warning for modern .NET targets.

## Team

Eyüp Karakaya and Kağan Kemal Üre
