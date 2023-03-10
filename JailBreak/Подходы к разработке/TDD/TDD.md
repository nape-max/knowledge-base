From: [[Подходы к разработке]]

> "Make it run, make it right"
> © Kent Block

Основные принципы TDD:
1) Новый код пишется только после того, как будет написан тест, завершающийся неудачей
2) Любое дублирование устраняется

Мантра TDD:
1) **Красный** - Перед написанием любого фрагмент кода - создайте тест, который будет терпеть неудачу или, возможно, даже не компилироваться
   ```php
   // ClassTest.php
   <?php
   
   class DollarTest
   {
	   public function TestMultiplier()
	   {
		   $class = new Dollar(5);
		   assert.equal(10, Dollar.multiply(2));
	   }
   }
   
   
   // Class.php
   <?php
   
   class Dollar
   {
	   public function multiply(): int
	   {
		   return 10;
	   }
   }
   
   
   ```
2) **Зеленый** - Напишите код, который заставить тест завершаться успехом, не думая о дизайне и чистоте кода. Напишите ровно столько кода, чтобы тест работал
3) **Рефаторинг** - Устраните любое дублирование в коде