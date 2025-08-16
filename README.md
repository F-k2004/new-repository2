# update_readme.py
import datetim
import random

quotes = [
    "امروز بهترین روز برای شروعه.",
    "با هر قدم، به هدفت نزدیک‌تر میشی.",
    "آرام ولی پیوسته حرکت کن.",
    "هر چالش فرصتی برای رشد است.",
    "تو توانایی انجامش رو داری!"
]

now = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
quote = random.choice(quotes)

content = f"""
# سلام! 👋

**زمان فعلی:** {now}

**نقل‌قول الهام‌بخش:**  
> {quote}
"""

with open("README.md", "w", encoding="utf-8") as f:
    f.write(content)

print("✅ فایل README.md با موفقیت به‌روز شد!")
