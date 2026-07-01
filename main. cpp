#include <iostream>
using namespace std;

// 1. بناء الكلاس (الكتالوج)
class Student {
private:
    string studentName; 
    double grade;       

public:
    // المُنشئ (Constructor)
    Student(string name) {
        studentName = name;
        grade = 0.0;
    }

    // دالة التعديل الآمنة (Setter) - البوابة الأمنية
    void setGrade(double newGrade) {
        if (newGrade >= 0 && newGrade <= 100) {
            grade = newGrade;
        } else {
            cout << "❌ خطأ أمني: الدرجة يجب أن تكون بين 0 و 100!" << endl;
        }
    }

    // دالة القراءة (Getter) للدرجة
    double getGrade() {
        return grade;
    }

    // دالة القراءة (Getter) للاسم
    string getName() {
        return studentName;
    }
};

// 2. الدالة الرئيسية لتشغيل النظام
int main() {
    // صناعة كائن واسمه rana (اخترنا اسمكِ!)
    Student rana("Rana");

    // محاولة إدخال درجة خاطئة (150)
    cout << "محاولة إدخال درجة 150..." << endl;
    rana.setGrade(150); 
    
    cout << "------------------------------------" << endl;

    // إدخال درجة صحيحة (98.5)
    cout << "محاولة إدخال درجة 98.5..." << endl;
    rana.setGrade(98.5);

    // طباعة البيانات المخزنة بأمان
    cout << "====================================" << endl;
    cout << "اسم الطالب: " << rana.getName() << endl;
    cout << "درجة الطالب: " << rana.getGrade() << "%" << endl;
    cout << "====================================" << endl;

    return 0;
}
