Guide to Using the SMS Management System:

This system is designed to use AT commands with a GSM module to receive, store, and manage SMS messages. Your code supports the following features:

    Receiving and Storing Messages:
        The system automatically receives incoming messages via Serial1 and stores them in a circular buffer.
        Incoming messages are checked for duplicates based on their timestamp to ensure uniqueness.

    Commands:
        sms: This command processes all messages stored in the buffer and displays their information, including phone number, message text, and timestamp.
        mas: This command displays the content of the messages.json file, containing details of all stored messages.
        del: This command clears the content of the messages.json file and replaces it with an empty JSON object.

    Scheduled Command Sending:
        The system automatically sends commands at set intervals (e.g., every 10 seconds) to check for new messages through the GSM module.

    Persian Language Support:
        The code includes a function for converting hexadecimal texts to Persian text, allowing Persian messages to be correctly displayed.

To use this system, you need to connect your GSM module to Serial1 and ensure your Arduino is correctly configured to communicate with the module. Also, make sure the LittleFS file system is properly initialized on your device to utilize the storage capabilities.

If you have any questions or need further assistance, please contact me at er.nasirian@gmail.com.


راهنمای استفاده از سیستم مدیریت پیام‌های کوتاه (SMS):

این سیستم با استفاده از دستورات AT برای ماژول GSM طراحی شده است تا بتواند پیام‌های SMS را دریافت، ذخیره‌سازی، و مدیریت کند. کد شما از ویژگی‌های زیر پشتیبانی می‌کند:

    دریافت و ذخیره پیام‌ها:
        سیستم به طور خودکار پیام‌های ورودی را از طریق Serial1 دریافت می‌کند و آن‌ها را در یک بافر دایره‌ای ذخیره می‌کند.
        پیام‌های دریافتی بر اساس زمان‌شان بررسی می‌شوند تا از تکراری نبودنشان اطمینان حاصل شود.

    کامندها:
        sms: این دستور تمام پیام‌های ذخیره‌شده در بافر را پردازش می‌کند و اطلاعات آن‌ها را نمایش می‌دهد. هر پیام شامل شماره تلفن، متن پیام، و زمان ارسال است.
        mas: این دستور محتوای فایل messages.json را نمایش می‌دهد، که شامل جزئیات تمام پیام‌های ذخیره‌شده است.
        del: این دستور محتوای فایل messages.json را پاک می‌کند و آن را با یک شیء JSON خالی جایگزین می‌کند.

    زمان‌بندی ارسال دستورات:
        سیستم به طور خودکار و در فواصل زمانی مشخص (مثلاً هر ۱۰ ثانیه) دستوراتی را برای بررسی پیام‌های جدید از طریق ماژول GSM ارسال می‌کند.

    پشتیبانی از زبان فارسی:
        کد شامل تابعی برای تبدیل متن‌های هگزادسیمال به متن فارسی است، که این امکان را فراهم می‌آورد تا پیام‌های فارسی به درستی نمایش داده شوند.

برای استفاده از این سیستم، شما باید ماژول GSM خود را به Serial1 متصل کنید و اطمینان حاصل نمایید که آردوینو شما برای ارتباط با این ماژول به درستی پیکربندی شده است. همچنین، مطمئن شوید که سیستم فایل LittleFS به درستی روی دستگاه شما راه‌اندازی شده است تا بتوانید از قابلیت‌های ذخیره‌سازی استفاده کنید.

اگر سوال یا نیاز به کمک بیشتری دارید، لطفاً با ایمیل er.nasirian@gmail.com با من تماس بگیرید.
