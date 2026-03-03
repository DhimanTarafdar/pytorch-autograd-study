# PyTorch Autograd Study Notebook

এই নোটবুকে আমি PyTorch এর Autograd নিয়ে আরও বিস্তারিতভাবে প্র্যাকটিস করেছি। এখানে বিভিন্ন ধরনের tensor নিয়ে কাজ করেছি এবং দেখেছি কিভাবে gradient ধাপে ধাপে calculate হয়।

এই ফাইলে আমি যেসব বিষয় নিয়ে কাজ করেছি:
- `requires_grad=True` ব্যবহার করে tensor তৈরি করা  
- `backward()` কল করে gradient বের করা  
- `grad` কিভাবে store হয় তা প্রিন্ট করে দেখা  
- কিছু ক্ষেত্রে কেন error আসে (যেমন requires_grad না দিলে) সেটা বোঝা  
- একাধিকবার backward() কল করলে gradient accumulate হয় কিনা সেটা observe করা  

এই নোটবুকটা আমি নিজের বোঝার সুবিধার জন্য তৈরি করেছি। এখানে আমি চেষ্টা করেছি PyTorch কিভাবে internally gradient হিসাব করে সেটা পরিষ্কারভাবে বুঝতে।
