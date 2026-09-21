SAGO STORE – SCALABLE FIREBASE STARTER

এই version-এ একসাথে সব product download হয় না। Customer ও Admin দুই জায়গাতেই 24টি করে pagination ব্যবহার করা হয়েছে। Search-এ nameLower দিয়ে prefix search করা হয়েছে। Image lazy loading আছে।

Firebase: Authentication Email/Password ON, Firestore চালু, admins/{OWNER_UID} document-এ role=owner রাখুন। Products-এ name, nameLower, categoryId, price, discountPrice, stock, imageUrl, description, active, createdAt, updatedAt রাখুন।

গুরুত্বপূর্ণ: কোটি কোটি product মানে unlimited/free নয়। Database size, indexes, traffic, reads/writes, image storage ও billing-এর ওপর capacity/cost নির্ভর করে। Firestore full-text search engine নয়; এই search prefix search। খুব বড় catalog হলে dedicated search service যোগ করা উচিত।

Firebase Storage এখানে ব্যবহার করা হয়নি; imageUrl ব্যবহার করুন। Storage billing চাইলে এখনই upgrade করার দরকার নেই। Payment secret key frontend-এ দেবেন না।

যদি Firebase index error দেখায়, Console-এর error link খুলে Create Index করুন।
