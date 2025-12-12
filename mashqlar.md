### **Mavzu 1: Klass nima va Ob'ekt yaratish**


1. **Shaxs klassi** - `Person` nomli klass yarating:
   - `name` (atribut) - ism
   - `age` (atribut) - yosh
   - `introduce()` (metod) - "Mening ismim [name], men [age] yoshdaman" deb chiqarish

2. **Mashina klassi** - `Car` nomli klass yarating:
   - `brand` (atribut) - markasi
   - `model` (atribut) - modeli
   - `year` (atribut) - yili
   - `start_engine()` (metod) - "Mashina yoqildi" deb chiqarish

3. **Kitob klassi** - `Book` nomli klass yarating:
   - `title` (atribut) - sarlavha
   - `author` (atribut) - muallif
   - `pages` (atribut) - sahifalar soni
   - `read()` (metod) - "Kitob o'qilyapti..." deb chiqarish

4. **Telefon klassi** - `Phone` nomli klass yarating:
   - `brand` (atribut) - brendi
   - `model` (atribut) - modeli
   - `battery` (atribut) - batareya foizi
   - `charge()` (metod) - batareyani 100% qilish

5. **Talaba klassi** - `Student` nomli klass yarating:
   - `name` (atribut) - ismi
   - `student_id` (atribut) - talaba ID si
   - `grades` (atribut) - baholar ro'yxati
   - `add_grade(grade)` (metod) - yangi baho qo'shish

---

### **Mavzu 2: Maxsus Metodlar (__init__, __str__)**


1. **Do'kon klassi** - `Store` nomli klass yarating:
   - `__init__()` metodida: `name`, `location`, `products` (bo'sh ro'yxat) o'rnating
   - `add_product(product)` - mahsulot qo'shish
   - `__str__()` - do'kon haqida ma'lumot chiqarish

2. **Bank Hisobi** - `BankAccount` nomli klass yarating:
   - `__init__()`: `owner`, `balance=0`
   - `deposit(amount)` - pul qo'shish
   - `withdraw(amount)` - pul yechish (balans yetmasa xabar)
   - `__str__()` - hisob ma'lumotlari

3. **To'do klassi** - `TodoList` nomli klass yarating:
   - `__init__()`: `tasks` (bo'sh ro'yxat)
   - `add_task(task)` - vazifa qo'shish
   - `complete_task(index)` - vazifa bajarildi deb belgilash
   - `__str__()` - barcha vazifalarni ko'rsatish

4. **O'yinchi klassi** - `Player` nomli klass yarating:
   - `__init__()`: `name`, `score=0`, `level=1`
   - `add_points(points)` - ball qo'shish
   - `level_up()` - darajani oshirish
   - `__str__()` - o'yinchi holati

5. **Mahsulot klassi** - `Product` nomli klass yarating:
   - `__init__()`: `name`, `price`, `quantity`
   - `discount(percent)` - chegirma qilish
   - `sell(amount)` - sotish (soni kamayadi)
   - `__str__()` - mahsulot ma'lumotlari

---

### **Mavzu 3: Asosiy Klassdan Meros olish**

1. **Hayvonlar ierarxiyasi**:
   - `Animal` nomli asosiy klass yarating: `name` atributi va `speak()` metodi bo'lsin
   - `Dog` klassini `Animal` dan meros oling: `speak()` metodini "Vov-vov!" qaytarish uchun override qiling
   - `Cat` klassini `Animal` dan meros oling: `speak()` metodini "Miyov!" qaytarish uchun override qiling

2. **Xodimlar ierarxiyasi**:
   - `Employee` nomli asosiy klass yarating: `name` va `salary` atributlari bo'lsin
   - `Manager` klassini `Employee` dan meros oling: `department` atributini qo'shing
   - `Developer` klassini `Employee` dan meros oling: `programming_language` atributini qo'shing

3. **Shakllar ierarxiyasi**:
   - `Shape` nomli asosiy klass yarating: `color` atributi va `area()` metodi bo'lsin
   - `Rectangle` klassini `Shape` dan meros oling: `width` va `height` atributlarini qo'shing, `area()` metodini width*height hisoblash uchun override qiling
   - `Circle` klassini `Shape` dan meros oling: `radius` atributini qo'shing, `area()` metodini 3.14*radius*radius hisoblash uchun override qiling

4. **Transport vositalari**:
   - `Vehicle` nomli asosiy klass yarating: `brand` va `model` atributlari, `start()` metodi bo'lsin
   - `Car` klassini `Vehicle` dan meros oling: `doors` atributini qo'shing
   - `Motorcycle` klassini `Vehicle` dan meros oling: `has_sidecar` atributini qo'shing

5. **Kitob turlari**:
   - `Book` nomli asosiy klass yarating: `title` va `author` atributlari bo'lsin
   - `Ebook` klassini `Book` dan meros oling: `file_size` atributini qo'shing
   - `PrintedBook` klassini `Book` dan meros oling: `pages` atributini qo'shing
   - `AudioBook` klassini `Book` dan meros oling: `duration` atributini qo'shing

---

### **Mavzu 4: Bir metod, ko'p shakl (Polimorfizm)**

1. **Ovoz chiqarish polimorfizmi**:
   - `Bird` nomli asosiy klass yarating: `make_sound()` metodi bo'lsin
   - `Duck` klassini `Bird` dan meros oling: `make_sound()` metodini "Quack quack" qaytarish uchun override qiling
   - `Sparrow` klassini `Bird` dan meros oling: `make_sound()` metodini "Chirp chirp" qaytarish uchun override qiling
   - `Owl` klassini `Bird` dan meros oling: `make_sound()` metodini "Hoot hoot" qaytarish uchun override qiling

2. **Hisoblash polimorfizmi**:
   - `Calculator` nomli asosiy klass yarating: `calculate(a, b)` metodi bo'lsin
   - `Adder` klassini `Calculator` dan meros oling: `calculate()` metodini a+b qaytarish uchun override qiling
   - `Subtractor` klassini `Calculator` dan meros oling: `calculate()` metodini a-b qaytarish uchun override qiling
   - `Multiplier` klassini `Calculator` dan meros oling: `calculate()` metodini a*b qaytarish uchun override qiling

3. **To'lov turlari polimorfizmi**:
   - `Payment` nomli asosiy klass yarating: `process_payment(amount)` metodi bo'lsin
   - `CashPayment` klassini `Payment` dan meros oling: `process_payment()` metodini override qiling
   - `CardPayment` klassini `Payment` dan meros oling: `process_payment()` metodini override qiling
   - `MobilePayment` klassini `Payment` dan meros oling: `process_payment()` metodini override qiling

4. **Ovqat tayyorlash polimorfizmi**:
   - `Chef` nomli asosiy klass yarating: `cook()` metodi bo'lsin
   - `PizzaChef` klassini `Chef` dan meros oling: `cook()` metodini override qiling
   - `PastaChef` klassini `Chef` dan meros oling: `cook()` metodini override qiling
   - `SushiChef` klassini `Chef` dan meros oling: `cook()` metodini override qiling

5. **Nashr qilish polimorfizmi**:
   - `Publisher` nomli asosiy klass yarating: `publish(content)` metodi bo'lsin
   - `NewspaperPublisher` klassini `Publisher` dan meros oling: `publish()` metodini override qiling
   - `MagazinePublisher` klassini `Publisher` dan meros oling: `publish()` metodini override qiling
   - `OnlinePublisher` klassini `Publisher` dan meros oling: `publish()` metodini override qiling

---

### **Mavzu 5: Kapsulyatsiya (Encapsulation)**

1. **Bank hisobi kapsulyatsiyasi**:
   - `BankAccount` klassini yarating: `_balance` (private atribut), `owner` (public atribut)
   - `deposit(amount)` metodi - balansga pul qo'shish
   - `withdraw(amount)` metodi - pul yechish (balans yetmasa xabar)
   - `get_balance()` metodi - balansni ko'rish

2. **Talaba baholari kapsulyatsiyasi**:
   - `Student` klassini yarating: `name` (public), `__grades` (private ro'yxat)
   - `add_grade(grade)` metodi - baho qo'shish (0-100 oralig'ida)
   - `get_average()` metodi - o'rtacha bahoni hisoblash
   - `get_grades()` metodi - barcha baholarni ko'rish

3. **Mahsulot narxi kapsulyatsiyasi**:
   - `Product` klassini yarating: `name` (public), `__price` (private), `__discount` (private)
   - `set_price(price)` metodi - narxni o'rnatish (manfiy bo'lmasligi kerak)
   - `apply_discount(percent)` metodi - chegirma qo'llash
   - `get_final_price()` metodi - yakuniy narxni hisoblash

4. **Foydalanuvchi paroli kapsulyatsiyasi**:
   - `User` klassini yarating: `username` (public), `__password` (private)
   - `set_password(new_password)` metodi - parol o'rnatish (kamida 8 belgi)
   - `check_password(input_password)` metodi - parolni tekshirish
   - `change_password(old_password, new_password)` metodi - parolni o'zgartirish

5. **Avtomobil benzin kapsulyatsiyasi**:
   - `Car` klassini yarating: `model` (public), `__fuel_level` (private 0-100)
   - `refuel(amount)` metodi - benzin quyish (100 dan oshmasligi kerak)
   - `drive(distance)` metodi - masofa bosish (benzin sarflanadi)
   - `get_fuel_level()` metodi - benzin darajasini ko'rish

---
