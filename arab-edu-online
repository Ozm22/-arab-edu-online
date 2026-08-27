<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>الأكاديمية العربيه للتعليم الإلكتروني</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'ozm-green': '#134e4a',
                        'ozm-gold': '#d97706',
                        'ozm-light': '#fdfbf7'
                    },
                    fontFamily: {
                        sans: ['Tajawal', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700;800&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Tajawal', sans-serif; background-color: #fdfbf7; }
        .hidden-step { display: none; }
    </style>
</head>
<body class="text-gray-800">

    <!-- شريط التنقل -->
    <nav class="flex justify-between items-center p-6 bg-white shadow-sm">
        <div class="flex gap-4 items-center">
            <button onclick="startRegistration()" class="bg-ozm-green text-white px-6 py-2 rounded-full font-bold hover:bg-teal-800 transition">انضم الآن</button>
            <button class="border border-ozm-gold text-ozm-gold px-6 py-2 rounded-full font-bold hover:bg-yellow-50 transition">تسجيل الدخول</button>
        </div>
        <ul class="hidden md:flex gap-6 font-semibold text-ozm-green">
            <li><a href="#">الرئيسية</a></li>
            <li><a href="#">الدورات</a></li>
            <li><a href="#">من نحن</a></li>
            <li><a href="#">المدونة</a></li>
            <li><a href="#">اتصل بنا</a></li>
        </ul>
        <div class="flex items-center gap-3">
            <h1 class="text-xl md:text-2xl font-extrabold text-ozm-green">الأكاديمية العربيه للتعليم الإلكتروني</h1>
            <div class="w-12 h-12 bg-ozm-green rounded-full flex items-center justify-center text-white font-bold text-xs text-center leading-tight">الأكاديمية<br>العربية</div>
        </div>
    </nav>

    <!-- الواجهة الرئيسية -->
    <main id="step-home" class="p-8 max-w-6xl mx-auto">
        <div class="relative rounded-3xl overflow-hidden shadow-2xl h-[500px]">
            <img src="1782141329597.png" alt="الواجهة الرئيسية" class="absolute inset-0 w-full h-full object-cover">
            <div class="absolute inset-0 bg-gradient-to-t from-ozm-green/90 to-transparent flex flex-col justify-end p-12 text-center">
                <h2 class="text-4xl md:text-5xl font-extrabold text-white mb-4">قيادة التميز المعرفي في العصر الرقمي</h2>
                <p class="text-lg text-gray-200 mb-8">بوابتك العربية إلى مستقبل واعد من التعليم الحديث والمهارات المتقدمة.</p>
                <div>
                    <button onclick="startRegistration()" class="bg-ozm-gold text-white px-8 py-3 rounded-full text-xl font-bold hover:bg-yellow-600 transition shadow-lg">ابدأ رحلتك التعليمية الآن</button>
                </div>
            </div>
        </div>
    </main>

    <!-- نموذج التسجيل التفاعلي -->
    <div id="registration-flow" class="hidden-step max-w-4xl mx-auto mt-10 bg-white p-8 rounded-2xl shadow-lg mb-20">
        
        <!-- الخطوة 1: نظام الدراسة -->
        <div id="step-1" class="step-container">
            <h3 class="text-2xl font-bold text-ozm-green mb-6 text-center">اختر نظام الدراسة</h3>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                <button onclick="selectSystem('diploma')" class="p-6 border-2 border-gray-200 rounded-xl hover:border-ozm-green hover:bg-teal-50 transition text-xl font-bold text-gray-700">دبلوم</button>
                <button onclick="selectSystem('bachelor')" class="p-6 border-2 border-gray-200 rounded-xl hover:border-ozm-green hover:bg-teal-50 transition text-xl font-bold text-gray-700">بكالوريوس</button>
                <button onclick="selectSystem('master')" class="p-6 border-2 border-gray-200 rounded-xl hover:border-ozm-green hover:bg-teal-50 transition text-xl font-bold text-gray-700">ماجستير</button>
            </div>
        </div>

        <!-- رسالة الماجستير -->
        <div id="step-master-soon" class="hidden-step text-center py-20">
            <h3 class="text-4xl font-bold text-ozm-green mb-4">قسم الماجستير</h3>
            <p class="text-2xl text-ozm-gold">قريباً.. انتظرونا!</p>
            <button onclick="goToStep('step-1')" class="mt-8 text-gray-500 underline">العودة</button>
        </div>

        <!-- الخطوة 2: المعلومات الشخصية -->
        <div id="step-2" class="hidden-step">
            <h3 class="text-2xl font-bold text-ozm-green mb-6 border-b pb-2">المعلومات الشخصية</h3>
            <form id="personal-info-form" class="grid grid-cols-1 md:grid-cols-2 gap-4">
                <input type="text" id="nameAr" placeholder="الاسم بالكامل (عربي)" class="border p-3 rounded w-full" required>
                <input type="text" id="nameEn" placeholder="الاسم بالكامل (إنجليزي)" class="border p-3 rounded w-full" required>
                <input type="email" id="email" placeholder="البريد الإلكتروني" class="border p-3 rounded w-full" required>
                <input type="text" id="nationality" placeholder="الجنسية" class="border p-3 rounded w-full" required>
                <input type="text" id="birthPlace" placeholder="مكان الميلاد" class="border p-3 rounded w-full" required>
                <input type="date" id="birthDate" class="border p-3 rounded w-full" required title="تاريخ الميلاد">
                <input type="text" id="passportNum" placeholder="رقم جواز السفر" class="border p-3 rounded w-full" required>
                <input type="date" id="passportIssue" class="border p-3 rounded w-full" required title="تاريخ الإصدار">
                <input type="date" id="passportExpiry" class="border p-3 rounded w-full" required title="تاريخ الانتهاء">
                <input type="number" id="gradYear" placeholder="سنة التخرج (الثانوية)" class="border p-3 rounded w-full" required>
                <input type="number" step="0.01" id="gradGPA" placeholder="معدل التخرج" class="border p-3 rounded w-full" required>
                <input type="text" id="certCode" placeholder="رقم الشهادة / رمز المعاملة" class="border p-3 rounded w-full" required>
                
                <div class="col-span-1 md:col-span-2 mt-4 bg-gray-50 p-4 rounded-lg border border-dashed border-gray-300">
                    <h4 class="font-bold text-gray-700 mb-2">المرفقات المطلوبة</h4>
                    <label class="block mb-2">جواز السفر: <input type="file" id="filePassport" class="mt-1 block w-full text-sm text-gray-500" required></label>
                    <label class="block">شهادة الثانوية (معمدة من الخارجية): <input type="file" id="fileCert" class="mt-1 block w-full text-sm text-gray-500" required></label>
                </div>
                
                <div class="col-span-1 md:col-span-2 flex justify-between mt-6">
                    <button type="button" onclick="goToStep('step-1')" class="px-6 py-2 bg-gray-200 text-gray-700 rounded-lg">رجوع</button>
                    <button type="button" onclick="validateStep2()" class="px-6 py-2 bg-ozm-green text-white rounded-lg font-bold">التالي: اختيار التخصص</button>
                </div>
            </form>
        </div>

        <!-- الخطوة 3: التخصص -->
        <div id="step-3" class="hidden-step">
            <h3 id="specialty-title" class="text-2xl font-bold text-ozm-green mb-2">اختيار التخصص</h3>
            <p id="specialty-rules" class="text-sm text-red-600 mb-6 font-semibold bg-red-50 p-3 rounded"></p>
            
            <div id="majors-container" class="grid grid-cols-1 md:grid-cols-2 gap-4">
            </div>
            <div class="flex justify-between mt-8">
                <button onclick="goToStep('step-2')" class="px-6 py-2 bg-gray-200 text-gray-700 rounded-lg">رجوع</button>
            </div>
        </div>

        <!-- الخطوة 4: الرسوم و طرق الدفع -->
        <div id="step-4" class="hidden-step">
            <h3 class="text-2xl font-bold text-ozm-green mb-6 border-b pb-2">تفاصيل الرسوم الدراسية وطريقة الدفع</h3>
            
            <div id="pricing-summary" class="bg-gray-50 p-6 rounded-xl border border-ozm-gold mb-8 shadow-sm">
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <div>
                    <label class="block font-bold text-gray-700 mb-2">الموطن الحالي لك:</label>
                    <select id="country" onchange="updatePaymentMethods()" class="border p-3 rounded w-full">
                        <option value="">اختر الدولة...</option>
                        <option value="السعودية">السعودية</option>
                        <option value="قطر">قطر</option>
                        <option value="البحرين">البحرين</option>
                        <option value="الكويت">الكويت</option>
                        <option value="العراق">العراق</option>
                        <option value="عمان">عمان</option>
                        <option value="اليمن">اليمن</option>
                        <option value="الأردن">الأردن</option>
                        <option value="مصر">مصر</option>
                        <option value="السودان">السودان</option>
                    </select>
                </div>
                <div>
                    <label class="block font-bold text-gray-700 mb-2">طريقة التحويل المناسبة:</label>
                    <select id="paymentMethod" class="border p-3 rounded w-full">
                        <option value="">اختر الدولة أولاً</option>
                    </select>
                </div>
                <div class="col-span-1 md:col-span-2">
                    <label class="block font-bold text-gray-700 mb-2">رقم الهاتف (للتواصل عبر واتساب/تلجرام):</label>
                    <input type="tel" id="phoneNumber" placeholder="مثال: +967 77..." class="border p-3 rounded w-full" required>
                </div>
            </div>

            <div class="flex justify-between mt-8">
                <button onclick="goToStep('step-3')" class="px-6 py-2 bg-gray-200 text-gray-700 rounded-lg">رجوع</button>
                <button onclick="submitForm()" class="px-8 py-3 bg-ozm-gold text-white rounded-lg font-bold text-lg shadow-md hover:bg-yellow-600 transition">تأكيد وإرسال الطلب</button>
            </div>
        </div>

        <!-- الخطوة 5: النجاح -->
        <div id="step-success" class="hidden-step text-center py-16">
            <div class="w-20 h-20 bg-green-100 text-green-600 rounded-full flex items-center justify-center text-4xl mx-auto mb-6">✓</div>
            <h3 class="text-3xl font-bold text-ozm-green mb-4">تم استلام طلبك بنجاح!</h3>
            <p class="text-lg text-gray-600 mb-2">سيتم مراجعة مرفقاتك والموافقة على الطلب في أقرب وقت.</p>
            <p class="text-lg text-gray-600 font-bold">سيتم الرد عليك بطريقة التحويل ورقم الحساب عبر الهاتف المسجل.</p>
            <p class="text-sm text-gray-400 mt-6">(تم الإرسال إلى المعرف @Eeaui)</p>
        </div>
    </div>

    <script>
        const data = {
            system: '',
            selectedMajor: '',
            tuitionInfo: {},
            majors: [
                'محاسبة', 'إدارة أعمال عربي', 'إدارة أعمال إنجليزي',
                'علوم حاسوب', 'ذكاء اصطناعي', 'جرافيكس', 'لغة إنجليزية', 'أمن سيبراني'
            ],
            pricing: {
                diploma: {
                    'محاسبة': 250, 'إدارة أعمال عربي': 250, 'إدارة أعمال إنجليزي': 350,
                    'علوم حاسوب': 350, 'ذكاء اصطناعي': 350, 'جرافيكس': 450, 'لغة إنجليزية': 350, 'أمن سيبراني': 450
                },
                bachelor: {
                    'محاسبة': 500, 'إدارة أعمال عربي': 500, 'إدارة أعمال إنجليزي': 650,
                    'علوم حاسوب': 650, 'ذكاء اصطناعي': 650, 'جرافيكس': 600, 'لغة إنجليزية': 650, 'أمن سيبراني': 600
                }
            },
            regFee: 50,
            emailFee: 25,
            terms: { diploma: 4, bachelor: 8 }
        };

        function hideAllSteps() {
            document.querySelectorAll('#registration-flow > div').forEach(el => el.classList.add('hidden-step'));
        }

        function goToStep(stepId) {
            hideAllSteps();
            document.getElementById(stepId).classList.remove('hidden-step');
            window.scrollTo({ top: document.getElementById('registration-flow').offsetTop - 20, behavior: 'smooth' });
        }

        function startRegistration() {
            document.getElementById('step-home').style.display = 'none';
            document.getElementById('registration-flow').classList.remove('hidden-step');
            goToStep('step-1');
        }

        function selectSystem(system) {
            data.system = system;
            if (system === 'master') {
                goToStep('step-master-soon');
            } else {
                goToStep('step-2');
            }
        }

        function validateStep2() {
            const form = document.getElementById('personal-info-form');
            if (form.checkValidity()) {
                generateMajors();
                goToStep('step-3');
            } else {
                form.reportValidity();
            }
        }

        function generateMajors() {
            const container = document.getElementById('majors-container');
            const rules = document.getElementById('specialty-rules');
            container.innerHTML = '';
            
            if (data.system === 'diploma') {
                document.getElementById('specialty-title').innerText = 'تخصصات قسم الدبلوم';
                rules.innerHTML = 'مدة الدبلوم 4 أترام (الترم شهرين).<br>عمر الشهادة الأقصى: 6 سنوات | العمر الأقصى للمتقدم: 35 سنة.';
            } else {
                document.getElementById('specialty-title').innerText = 'تخصصات قسم البكالوريوس';
                rules.innerHTML = 'مدة الدراسة 8 أترام (الترم شهرين).<br>عمر الشهادة الأقصى: 4 سنوات | العمر الأقصى للمتقدم: 28 سنة.';
            }

            data.majors.forEach(major => {
                const btn = document.createElement('button');
                btn.className = 'p-4 border border-gray-300 rounded-lg text-right font-bold hover:bg-ozm-green hover:text-white transition shadow-sm';
                btn.innerText = major;
                btn.onclick = () => selectMajor(major);
                container.appendChild(btn);
            });
        }

        function selectMajor(major) {
            data.selectedMajor = major;
            calculatePricing();
            goToStep('step-4');
        }

        function calculatePricing() {
            const tuition = data.pricing[data.system][data.selectedMajor];
            const termCount = data.terms[data.system];
            const total = tuition + data.regFee + data.emailFee;
            const perTerm = (total / termCount).toFixed(2);

            const summaryHtml = `
                <h4 class="text-xl font-bold text-ozm-green mb-4">التخصص المختار: ${data.selectedMajor} (${data.system === 'diploma' ? 'دبلوم' : 'بكالوريوس'})</h4>
                <ul class="space-y-3 text-lg">
                    <li class="flex justify-between border-b pb-2"><span>رسوم التسجيل:</span> <span>$${data.regFee}</span></li>
                    <li class="flex justify-between border-b pb-2"><span>رسوم إنشاء إيميل جامعي:</span> <span>$${data.emailFee}</span></li>
                    <li class="flex justify-between border-b pb-2 font-bold"><span>الرسوم الدراسية الكلية للتخصص:</span> <span>$${tuition}</span></li>
                    <li class="flex justify-between border-b border-ozm-gold pb-2 mt-4 text-ozm-green font-extrabold text-xl">
                        <span>إجمالي المبلغ المطلوب:</span> <span>$${total}</span>
                    </li>
                    <li class="flex justify-between pt-2 text-ozm-gold font-bold">
                        <span>المبلغ المستحق لكل ترم (${termCount} أترام):</span> <span>$${perTerm} / ترم</span>
                    </li>
                </ul>
            `;
            document.getElementById('pricing-summary').innerHTML = summaryHtml;
        }

        function updatePaymentMethods() {
            const country = document.getElementById('country').value;
            const methodSelect = document.getElementById('paymentMethod');
            methodSelect.innerHTML = '';
            
            let methods = [];
            if (country === 'اليمن') methods = ['الكريمي', 'النجم', 'بنك التضامن'];
            else if (country === 'السعودية') methods = ['STC Pay', 'تحويل بنكي (الراجحي)', 'ويسترن يونيون'];
            else if (country === 'مصر') methods = ['فودافون كاش', 'إنستا باي', 'ويسترن يونيون'];
            else methods = ['ويسترن يونيون', 'موني جرام', 'تحويل بنكي دولي'];

            methods.forEach(m => {
                const opt = document.createElement('option');
                opt.value = m;
                opt.innerText = m;
                methodSelect.appendChild(opt);
            });
        }

        async function submitForm() {
            const phone = document.getElementById('phoneNumber').value;
            const country = document.getElementById('country').value;
            if (!phone || !country) {
                alert('يرجى تعبئة الدولة ورقم الهاتف.');
                return;
            }

            const studentName = document.getElementById('nameAr').value;
            const message = `
🌟 طلب تسجيل جديد - الأكاديمية العربيه للتعليم الإلكتروني 🌟
الاسم: ${studentName}
النظام: ${data.system}
التخصص: ${data.selectedMajor}
الدولة: ${country}
الهاتف: ${phone}
طريقة الدفع المطلوبة: ${document.getElementById('paymentMethod').value}
            `;
            
            goToStep('step-success');
        }
    </script>
</body>
</html>
