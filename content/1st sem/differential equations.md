---
cssclasses:
  - rtl-note
---
#1stSem #mathmatics
# مراجعة علي القديم
(اياك وثابت التكامل)

$$
\begin{array}{c | l}
   g(x) &  \int g(x) \, dx \\[1ex]
   \hline
   \dfrac{f'(x)}{\sqrt{a^2 - f^2(x)}} & 
   \displaystyle\sin^{-1}\left(\frac{f(x)}{a}\right) + C \quad \text{or} \quad -\cos^{-1}\left(\frac{f(x)}{a}\right) + C \\[2.5ex]
   
   \dfrac{f'(x)}{a^2 + f^2(x)} & 
   \displaystyle\frac{1}{a} \tan^{-1}\left(\frac{f(x)}{a}\right) + C \quad \text{or} \quad -\frac{1}{a} \cot^{-1}\left(\frac{f(x)}{a}\right) + C \\[2.5ex]
   
   \dfrac{f'(x)}{f(x)\sqrt{f^2(x) - a^2}} & 
   \displaystyle\frac{1}{a} \sec^{-1}\left(\frac{f(x)}{a}\right) + C \quad \text{or} \quad -\frac{1}{a} \text{cosec}^{-1}\left(\frac{f(x)}{a}\right) + C \\[2.5ex]
   \hline
   \dfrac{f'(x)}{\sqrt{a^2 + f^2(x)}} & 
   \displaystyle\sinh^{-1}\left(\frac{f(x)}{a}\right) + C \\[2.5ex]

   \dfrac{f'(x)}{\sqrt{f^2(x) - a^2}} & 
   \displaystyle\cosh^{-1}\left(\frac{f(x)}{a}\right) + C \\[2.5ex]

   \dfrac{f'(x)}{a^2 - f^2(x)} & 
   \displaystyle\frac{1}{a} \tanh^{-1}\left(\frac{f(x)}{a}\right) + C \quad \text{or} \quad \frac{1}{a} \coth^{-1}\left(\frac{f(x)}{a}\right) + C \\[2.5ex]

   \dfrac{f'(x)}{f(x)\sqrt{a^2 - f^2(x)}} & 
   \displaystyle-\frac{1}{a} \text{sech}^{-1}\left(\frac{f(x)}{a}\right) + C \\[2.5ex]

   \dfrac{f'(x)}{f(x)\sqrt{a^2 + f^2(x)}} & 
   \displaystyle-\frac{1}{a} \text{cosech}^{-1}\left(\frac{f(x)}{a}\right) + C 
\end{array}
$$

# الباب الأول: مقدمة (Introduction)
## تعريفات
### معادلة تفاضلية عادية (ordinary differential equation ODE):
تكون دالة في متغير مستقل واحد:   $y = f(x)$
وjكون المشتقات: 

$$
y = y ^{(0)} \quad,\quad y' = \frac{dy}{dx} \quad,\quad y'' = \frac{d^2y}{dx^2} \quad,\quad \cdots \quad,\quad y ^{(n)} = \frac{d^ny}{dx^n}
$$

### معادلة تفاضلية جزئية (partial differential equation PDE):#
تكون دالة في اكثر من متغير:   $z = f(x,y)$
وjكون المشتقات: 

$$
z = z ^{(0)} \quad,\quad \frac{\partial z}{dx} \;,\; \frac{\partial z}{dy} \;,\; \frac{\partial^2 z}{dx^2} \;,\; \frac{\partial^2 z}{dy^2} \;,\; \frac{\partial^2 z}{dxy}
$$

### أنواع المعادلات التفاضلية
#### خطية linear:
1. المتغير التابع وجميع مشتقاته من *الدرجة الأولى* فقط
2. المتغير التابع وجميع مشتقاته *ليست كحواصل ضرب*
#### غير خطية non-linear:
ما ليس معادلة خطية#
### رتبة المعادلة التفاضلية
اعلى معامل تفاضلي يظهر في المعادلة التفاضلية **(أعلى مشتقة)**

 $x(y'')^2 + 6y' = e^x + y^{(4)}$ *(رتبة رابعة)*

 $\dfrac{\partial u}{\partial x} + \dfrac{\partial u}{\partial t} \dfrac{\partial^2 u}{\partial x^2} - \dfrac{\partial^3 u}{\partial x^2 \partial t} = x e^t \sin t$ *(رتبة ثالثة)*
### درجة المعادلة التفاضلية
هي القوة المرفوعة إليها أعلى مشتقة تفاضلية في المعادلة بعد وضعها في الصورة الجذرية الصحيحة **(أس أعلى مشتقة)**
$(y''')^5 + (y')^2 = y y'$ *(درجة خامسة)*

$(y'' + 1)^{\frac{1}{2}} = x^2 - {y'}^2 \;\Rightarrow\; (y'' + 1) = (x^2 - {y'}^2)^2$ *(درجة اولى)*

## تكوين المعادلة التفاضلية

$$
f(x,y,c_1,c_2,\cdots,c_n) \Rightarrow f(x,y,y',\cdots,y^{(n)})
$$

1. نحدد عدد الثوابت الاختيارية في المسئلة
2. تفاضل المعادلة بنفس عدد الثوابت
3. نستخدم المعادلات السابقة لحذف الثوابت
## حل المعادلة التفاضلية
### حل عام
حل به ثوابت اختيارية, بنفس رتبة المعادلة
### حل خاص
هو الحل العامل بعد وضع الثوابت الاختيارية (بعضهما او كلاهما) بقيم عددية (تعويض في الثوابت)
### حل شاذ/مفرد
حل لا يمكن استنتاجه من الحل العام او الخاص
# الباب الثاني: معادلات تفاضلية من الرتبة الأولى والدرجة الأولى
متنساش ثابت التكامل
## 1-معادلة قابلة لفصل متغيراتها "Equations with separable variables"
الصورة العامة:

$$
\color{#a7c957}\large  p_1(x)\,p_2(y)\,dx +q_1(x)\,q_2(y)\,dy = 0
$$

حيث ان $p : p(x,\,y) \quad,\quad q : q(x,\,y)$

فانه بمكن فصل كل متغير على حذة ويكون الحل العام للمعادلة هو:

$$
\int \dfrac{p_1(x)}{q_1(x)}dx \,+ \int \dfrac{p_2(y)}{q_2(y)}dy = c
$$

حيث c ثابت اختياري
### ملاحظة
تذكر ان $y' = dy/dx$ , فإذا كانت المعادلة علي الشكل:

$$
p(x,\,y) +  q(x,\,y)y' = 0
$$

بالتأثير بـ(dx) علي المعادلة ( ايوة بنضرب بـ(dx) بس قولها في دماغك مش الورقة ):

$$
p(x,\,y)dx +  q(x,\,y)dy = 0
$$

## 2-المعادلات المتجانسة "Homogeneous equations"
#### تكون الدالة متجانسة من الدرجة n اذا كان:

$$
p(\lambda x, \lambda y) = \lambda^n\;p(x,y)
$$

مثلا: $x^2 dx + xy\,dy + y^2 dy = 0$ معادلة متجانسة من الدرجة التانية
(يعني مجموع رتب x و y في كل حد متساوية)
### خطوات
#### 1. تأكد أن المعادلة متجانسة
#### 2. وضع المعادلة في الصورة $\dfrac{dy}{dx} = f\left(\dfrac{y}{x}\right)$ 
#### 3. بفرض:
 
$$
u = \dfrac{y}{x} \quad,\quad y = ux \quad,\quad \dfrac{dy}{dx} = x\dfrac{du}{dx} + u
$$

#### 4. فصل المتغيرات  والتكامل والتعويض بـ $u = \dfrac{y}{x}$
 
$$
\begin{array}{c}
 \dfrac{dy}{dx} = f\left(\dfrac{y}{x}\right) \quad\rightarrow\quad x\,\dfrac{du}{dx} + u= f(u) \quad\rightarrow\quad x\,\dfrac{du}{dx} = f(u) - u \\
 \Rightarrow \dfrac{du}{f(u)-u} = \dfrac{dx}{x}
 \end{array}
$$

 
## 3-المعادلات ذات المعاملات الخطية "Equations with linear coefficients":
#### الصورة العامة:

$$
\large\left( a_1 x + b_1y + c_1 \right)dx + \left( a_2 x + b_2 y + c_2 \right)dy = 0
$$

- لاحظ انه عند:  $c_1 = c_2 = 0$ , تكون **معادلة متجانسة** ويمكن حلها بالطريقة السابقة
- اذا كان احد المتغيران لا يساوي صفر, تصبح معادلة غير متجانسة ويكون حلها في شكل المستقيمين
### المستقيمان متقاطعان

$$
\color{#acffcc}\large \large\dfrac{a_1}{a_2} \ne \dfrac{b_1}{b_2}
$$

فإن المستقيمان يتقاطعان في نقطة $(h,k)$
#### نوجد حل المعادلتان:

$$
\begin{array}{c} a_1 x + b_1y + c_1 =0 \\ a_2 x + b_2 y + c_2 = 0 \end{array}
$$

#### بفرض التعويض:

$$
\begin{array}{l}
x = X + h &,& y = Y+k \\
dx = dX &,& dy = dY
\end{array}
$$

#### ينعدم الحدان الثابتان وتصبج المعادلة:

$$
(a_1 X + b_1 Y)\,dX + (a_2 X + b_2 Y)\,dY = 0
$$

وهذه معادلو متجانسة في $X,Y$
### المستقيمان متوازيان

$$
\color{#acffcc}\large\dfrac{a_1}{a_2} = \dfrac{b_1}{b_2} = \dfrac 1 m
$$

#### إذن يكون:

$$
a_2\,x + b_2\,y= m(a_1 x + b_1 y)
$$

#### بفرض:

$$
\begin{array}{l}
z = a_1\,x + b_1\,y\\
dz = a_1\,dx + b_1\,dy
\end{array}
$$

بالتعويض في المعادلة الاصلية تصبح معادلة تفاضلية قابلة للفصل
## 4-المعادلة التفاضلية التامة "Exact differential equations":

$$
\color{#a7c957}\large \large p(x,y)\,dx + q(x,y)\,dy = 0
$$

#### الشرط الضروري والكافي لكي تكون المعادلة تامة هو:

$$
\dfrac{\partial p}{\partial y} = \dfrac{\partial q}{\partial x}
$$

#### بفرض وجود دالة $u$ حيث : 

$$
du = p\,dx + q\,dy
$$

اذا تحقق الشرط, يمكن تكامل المعادلة الاساسية للحصول علي  $u = C$ 
غالبا بتبقي الدالة ناتج اشتقاق دالتين, حاول تركز علي حاصل ضرب دالتين عند اشتقاقهم بتنتج المعادلة التامة
### مثال

$$
\begin{array}{l}
\large\color{#acffcc}\ln(1+y^2)\,dx + \dfrac{2y(x-1)}{y^2+1}\,dy = 0 \\[2.5px]
p(x,y) = ln(1+y^2) \;\rightarrow\; \dfrac{\partial p}{\partial y} = \dfrac{2y}{1+y^2} \\[2.5px]
q(x,y) = \dfrac{2y(x-1)}{y^2+1} \;\rightarrow\; \dfrac{\partial q}{\partial x} = \dfrac{2y}{1+y^2} \\
\text{}
\end{array}
$$

## 5-المعادلة التفاضلية الخطية "Linear differential equations"
#### الصورة العامة:

$$
\color{#a7c957}\large \large\dfrac{dy}{dx} + f(x)\,y = g(x)
$$

#### لحل المعادلة, أولا نوجد العامل المكامل:

$$
\large\mu = e^{\,\int\!f(x)dx}
$$

#### يكون حل المعادلة:

$$
y\,\mu = \int\mu\,g(x)dx
$$

### ملاحظة:
اذا كانت المعادلة:

$$
h(x)\dfrac{dy}{dx} + f(x)\,y = g(x)
$$

فيمكن قسمة المعادلة علي $h(x)$ وتصبح المعادلة في الصورة الصحيحة
اما اذا كانت $h(y)$ فيجب تغير شكل المعادلة لأنها ليست خطية
*غالبا بيبقي فيه دالة تانية في $y$ مع $f(x)$ عشان تاخد تعويض وتتحول الدالة وتبقي المعادلة خطية*

$$
h(y)\dfrac{dy}{dx} + f(x)\,k(y) = g(x)
$$

$$
u = k(y) \quad,\quad \dfrac{du}{dx} = k' (y) = h(y) \dfrac{dy}{dx}
$$

$$
\dfrac{du}{dx} + f(x)u = g(x)
$$

 *بس مش شرط, ممكن متجيش كدة. الفكرة بس متكررة*
## 6- معادلات برنولي "Bernoulli's equation" :

$$
\color{#a7c957}\large \dfrac{dy}{dx} + f(x)\,y = g(x)\,y^n
$$

حيث $n$ عدد حقيقي
#### لاحظ انه:
- عند $n=1$ تكون المعادلة: $\large\dfrac{dy}{dx} + \left( f(x) - g(x) \right)\,y = 0$ وهي معادلة قابلة للفصل
- عند $n=0$ تكون المعادلة: $\large\dfrac{dy}{dx} + f(x)\,y = g(x)$ وهي معادلة خطية
### خطوات
#### 1. بقسمة المعادلة على $y^n$ 
$$
y^{-n} \dfrac{dy}{dx} + f(x)\,y^{1-n} = g(x)
$$

#### 2. بفرض: 
$$
u = y^{1-n} \quad,\quad \dfrac{du}{dx} = (1-n)\,y^{-n}\dfrac{dy}{dx}
$$

#### 3. بالتعويض:

$$
\dfrac{dy}{dx} + (1-n)f(x)\,u = (1-n)\,g(x)
$$

تصبح معادلة خطية في $u$ يمكن حلها
متنساش تعوض تاني بـ $u = y^{1-n}$ 
# الباب الثالث: معادلات تفاضلية رتبة اولى ودرجات عليا
حيث ان $C_1$ ثابت تكامل اختياري

#### الصورة العامة:

$$
\color{#a7c957}\large \large L_{0}(x,y) \, p^{n} + L_{1}(x,y) \, p^{n-1} + \cdots+L_{n-1}(x,y)\,p + L_{n}(x,y) =0
$$

حيث:
-  $p=\dfrac{dy}{dx}$
-  $L_0 \; , L_1 \; , \cdots , L_n$ دوال متغيرة في x , y
## 1-المعادلات القابلة للحل في p :
يمكن اعتبار المعادلة التفاضلية كمعادلة جبرية في $p$ وإيجاد جزورها على الصورة:

$$
\large(p-m_1)\,\cdot\,(p-m_2)\,\cdots\,(p-m_n)=0
$$

#### عند حل المعادلات:

$$
\begin{array}{c|c|c|r}
p-m_1 = 0 & p-m_2 = 0 & p-m_n = 0 & (1 \\
\dfrac{dy}{dx} = m_1(x,y) & \dfrac{dy}{dx} = m_2(x,y) & \dfrac{dy}{dx} = m_n(x,y) & (2\\[2.5px]
\Downarrow & \Downarrow & \Downarrow \\[2.5px]
f_1(x,y,c_1) = 0 & f_2(x,y,c_2) = 0 & f_n(x,y,c_n) = 0 & (3
\end{array}
$$

#### يصبح الناتج علي شكل: 

$$
\large f_1(x,y,c_1)\,\cdot\,f_2(x,y,c_2)\,\cdots\,f_n(x,y,c_n)=0
$$

## 2-معادلات قابلة للحل في x
عا
## 3-معادلات قابلة للحل في y

$$
\color{#a7c957}\large y = f(x,p) \qquad (1)
$$

#### عند تفاضل الطرفين بالنسبة لـ $x$ :

$$
\dfrac{dy}{dx} = p = \dfrac{\partial f}{\partial x} + \dfrac{\partial f}{\partial p}\cdot\dfrac{\partial p}{\partial x}
$$

وهذه معادلة تفاضلية في $x,p$ يمكن حلها بفصل المتغيرات والتكامل للحصول على الصورة:

$$
x = \phi(p,c) \qquad (2)
$$

#### بالتعويض في المعادلة $(1)$ نحصل على:

$$
y = \psi (p,c) \qquad (3)
$$

والمعادلتان $(2) , (3)$ معادلتان بارامتريتان.
الحل العام للمعادلة $(1)$ **ينتج من حذف $p$** بين المعادلتان, إذا تعذر الحذف **فنكتفي بالصورة البارامترية** للحل
## 4- معادلة كليروت "Clairaut's equation":

$$
\color{#a7c957}\large y = p\,x + f(p)
$$

*لاحظ انها معادلة قابلة للحل في y*

$$
\begin{array}{c}
	p = p+x \dfrac{dp}{dx} + f'(p) \dfrac{dp}{dx}\\
	\{x+f'(p)\} \dfrac{dp\,}{dx} = 0\\[5px]
	\hline
	\begin{array}{l|l}
		(1) & (2) \\[2.5px]
		\dfrac{dp}{dx} = 0 & x+f(p) = 0\\[2.5px]
		\therefore \; p = c & \therefore \; x = -f'(p)\\
		\rightarrow y = cx + f(c) & \rightarrow y = -f'(p)\,p + f(p)
	\end{array}
\end{array}
$$

تكون المعادلتان  $(1) , (2)$ معادلتان بارامتريتان ويمكن حذف $p$ منهمل للحصول علي علاقة بين  $x,y$ علي صورة $\Phi(x,y)=0$
# الباب الخامس: معادلات تفاضلية خطية ذات معاملات ثابتة
<p style = "text-align: right">you know the drill</p>

#### الصورة العامة:

$$
\color{#a7c957}\large a_0 \dfrac{d^n y}{dx^n} + a_1 \dfrac{d^{n-1} y}{dx^{n-1}} + \cdots+a_{n-1} \dfrac{dy}{dx} + a_n\,y = \phi(x)\\[2.5px]
$$

$$
\color{#00ffb3}\text{assume: } D = \dfrac{d}{dx} \quad,\quad D^2 = \dfrac{d^2}{dx^2} \quad,\quad D^n = \dfrac{d^n}{dx^n}
$$

$$
\color{#a7c957}\large\left(a_0\,D^n + a_1\,D^{n-1} + \cdots + a_{n-1}\,D + a_n \right)y = \phi(x)\\[7.5px]
$$

$$
\color{#a7c957}\large f(D)y = \phi(x)
$$

## الحل العام منقسم الى شقين
### الحل المكمل:

$$
y_c:f(D)y = 0
$$

### الحل الخاص:

$$
y_p:f(D)y = \phi(x)
$$

### الحل العام:

$$
\large y = y_c + y_p
$$

## خطوات الحل (المكمل):
#### 1. فرض:

$$
\large y = e^{mx} \quad,\quad y' = m\,e^{mx} \quad,\quad y^{(n)} = m^n\,e^{mx}
$$

#### 2. بالتعويض في المعادلة والقسمة علي $e^{mx}$ :

$$
a_0\,m^n + a_1\,m^{n-1} + \cdots + a_n = 0
$$

وهي معادلة جبرية من الدرجة n
#### 3. على حسب نوع الجذور يتم تحديد الحل:

$$
\large\begin{array}{l|l}
	m_1 \ne m_2 \ne m_3 \ne \cdots & y_c = c_1\,e^{m_1\,x} + c_2\,e^{m_2\,x} + \cdots \\
	m_1 = m_2 = m_3 =\cdots & y_c = c_1\,e^{m_1\,x} + c_2\,xe^{m_2\,x} + c_3\,x^2e^{m_3\,x} + \cdots \\[8px]
	\begin{array}{l}
	m_{1,2} = \alpha_1 \pm \beta_1 i \\
	m_{3,4} = \alpha_2 \pm \beta_2 i \\
	\end{array}
	&
	\begin{array}{l}
	y_c = e^{\alpha_1 x}\left[c_1 \sin \beta_1 x + c_2 \cos \beta_1 x \right]\\[5px]
	\quad +\, e^{\alpha_2\,x}\left[c_3 \sin \beta_2\,x + c_4 \cos \beta_2\,x \right]
	\end{array}
	\\[8px]
	m_{1,2} = m_{3,4}= \alpha \pm \beta i &
	\begin{align}
	y_c &= e^{\alpha x}\left[c_1 \sin \beta x + c_2 \cos \beta x \right]\\[5px]
	&+xe^{\alpha x}\left[c_3 \sin \beta x + c_4 \cos \beta x \right]
	\end{align}
	\\[8px]
\end{array}
$$

## خطوات الحل (الخاص):

$$
f(D)y = \phi(x) \quad\rightarrow\quad y = \dfrac{1}{f(D)}\left\{\phi (x)\right\}
$$

حيث أن $\dfrac 1 D$ يعادل عملية التكامل
### الحالة الاولى: دالة أسية $\phi(x) = e^{mx}$ :

$$
D\,e^{mx} = m\,e^{mx}\quad\Rightarrow D=m \quad\Rightarrow f(D) = f(m)
$$

$$
y_p = \dfrac{1}{f(D)}\{e^{mx}\} = \dfrac{1}{f(m)}\{e^{mx}\}\qquad\text{for: } f(m) \ne0
$$

$$
y_p = \dfrac{x^{(r)}}{f^{(r)}(m)}\{e^{mx}\}\qquad\text{for: } f(m)=0
$$

حيث المشتقة $r$ هي التي لا تعطي صفر في المقام
#### إذا كانت $\phi(x) =C$ فيمكن الحل بالدالة الأسية على أساس أن $m = 0$ 
### الحالة الثانية: دالة مثلثية $\phi(x) = \sin(ax+b) \text{ or } \cos(ax+b)$ : 

$$
D\{ \sin(ax+b) \} = a\cos(ax+b)
$$

$$
D^2\{ \sin(ax+b) \} = -a^2\sin(ax+b)
$$

$$
\text{same for }[\cos(ax+b)] \Rightarrow \color{#00ffb3}D^2 = -a^2
$$

حاول جعل $f(D^2) \leftarrow f(D)$ ثم استخدم التعويض المذكور
*إذا تبقي حد فردي في المقام:* قم بضرب المعادلة في المرافق:

$$
\begin{align}
f(D) &= \dfrac{1}{a_1D+b_1} = \dfrac{1}{a_1D+b_1} \cdot \dfrac{a_1D-b_1}{a_1D-b_1}\\[5px]
&= \dfrac{a_1D-b}{a_1^2D^2-b_1^2} = \dfrac{a_1D-b_1}{a_1^2(-a^2) - b_1^2}
\end{align}
$$

هكذا يمكن اشتقاق الدالة والحصول على الحل الخاص
#### في حالة ان المقام يساوي صفر
تذكر أن

$$
\large e^{i\,mx} = \cos mx + i\sin mx
$$

يتم تحويل المعادلة الي الصورة الأسية:

$$
\begin{array}{l}
\dfrac{1}{f(D)}\{\sin mx\} = Im\left[ \dfrac{1}{f(D)}\{ e^{i\,mx} \} \right]\\
\dfrac{1}{f(D)}\{\cos mx\} = Re\left[ \dfrac{1}{f(D)}\{ e^{i\,mx} \} \right]\\
\end{array}
$$

ويتم حل المعادلة **بالحالة الأولى**
### الحالة الثالثة: كثيرات حدود

$$
\color{#acffcc}\large\phi(x) = A_0\,x^{r_1} + A_1\,x^{r_1-1} + \cdots + A_{r_1-1}x + A_{r_1}
$$

يوجد طريقاتان للحل
#### ذات الحدين
تذكر أن:

$$
\color{#00ffb3}(1+x)^n \color{#f7ecc2} = 1 + nx + \dfrac{n(n-1)}{2!} x^2 + \dfrac{n(n-1)(n-2)}{3!} x^3 + \cdots
$$

$$
\color{#00ffb3}(a+x)^n \color{#f7ecc2}= a^n (1+\dfrac{x}{a})^n = 1 + n\dfrac{x}{a} + \dfrac{n(n-1)}{2!} \left(\dfrac{x}{a}\right)^2 + \cdots
$$

$$
\color{#00ffb3}(1+x)^{-1}\color{#f7ecc2} = 1 - x + x^2 - x^3 + \cdots
$$

$$
\color{#00ffb3}(1-x)^{-1}\color{#f7ecc2} = 1 + x + x^2 + x^3 + \cdots
$$

1. تحليل دالة المقام الى أبسط صورة (يفضل درجة أولى إذا أمكن):

$$
\begin{align}
y_p = \dfrac{1}{f(D)} &= \dfrac{1}{b_1D + c_1} \cdot \dfrac{1}{b_2D + c_2} \cdots \dfrac{1}{b_nD + c_n}\\[2.5px]
&= (b_1D + c_1)^{-1} \cdot (b_2D + c_2)^{-1} \cdots (b_nD + c_n)^{-1} 
\end{align}
$$

2. استخدام مفكوك ذات الحدين (آخر معادلتين) لكل قوس حده
3. ضرب الأقواس للحصول علي درجة $r_1$
#### المعاملات غير المعينة
بفرض أن

$$
\large y = x^{r_2} [a_0\,x^{r_1} + a_1\,x^{r_1-1} + \cdots +a_{r_1}]
$$

حيث أن $r_2$ اصغر مشتقة تظهر في المعادلة ( أصفر أس لـ $D$ )
يتم إشتقاق $(r_1-1)$ مرة وجمع الحدود ومقارنة المعاملات للحصول علي حل
**مثلا**:

$$
\large\begin{array}{l}
(D^2 + 2D + 2)y = 2x^3 +2\\
r_1 = 3 \quad,\quad r_2 = 0\\
y = a_0\,x^3 + a_1\,x^2 + a_2\,x + a_3\\
y' = 3a_0\,x^2 + 2a_1\,x + a_2\\
y'' = 6a_0\,x + 2a_1\\
y'' + 2y' + 2y = 2x^3 + 2
\end{array}
$$

### قانون الإزاحة
اذا كانت $\phi(x)$ حاصل ضرب دالتين وكانت واحدة منهم دالة أسية أو مثلثية, فيمكن إخراجها من المؤثر العكسي $\dfrac{1}{f(D)}$  كالتالي:

$$
\large y_p = \dfrac{1}{f(D)}\{e^{mx} Z{(x)}\} = \dfrac{e^{mx}}{f(D+m)}\{ Z{(x)}\}
$$

$$
\large y_p = \dfrac{1}{f(D)}\left\{\sin (ax) Z{(x)}\right\} = Im\left[\dfrac{1}{f(D)}\{e^{i\,ax} Z{(x)}\}\right] = Im\left[\dfrac{e^{i\,ax}}{f(D+ia)}\{ Z{(x)}\}\right]
$$

$$
\large y_p = \dfrac{1}{f(D)}\left\{\cos (ax) Z{(x)}\right\} = Re\left[\dfrac{1}{f(D)}\{e^{i\,ax} Z{(x)}\}\right] = Re\left[\dfrac{e^{i\,ax}}{f(D+ia)}\{ Z{(x)}\}\right]
$$

# الباب السادس: معادلات تفاضلية خطية ذات معادلات متغيرة
## معادلة اويلر الخطية
تكون معادلة بها $x$ و $D$ لكل حد مرفوع لنفس الدرجة $n$  

$$
\color{#a7c957}\large\left(a_0\,x^n D^n + a_1\,x^{n-1} D^{n-1} + \cdots + a_{n-1}\,xD + a_n 
\right)y = \phi(x)\\[7.5px]
$$

### الحل
#### 1.نفرض أن:

$$
x = e^t \;,\quad \dfrac{dx}{dt} = e^t \;,\quad \dfrac{dt}{dx} = e^{-t} = \dfrac 1 x
$$

$$
\begin{array}{l}
\dfrac{dy}{dx} = \dfrac{dy}{dt} \cdot \dfrac{dt}{dx} = D_1 \cdot \dfrac 1 x &\Rightarrow xD = D_1\\[2.5px]
\dfrac{d^2}{dx^2} = \dfrac{1}{x^2}D_1(D_1-1) &\Rightarrow x^2D^2 = D_1 (D_1-1)\\
\end{array}
$$

#### 2.ومنه نستنتج:

$$
\begin{array}{l}
 xDy = D_1y\\
x^2 D^2 y= D_1 (D_1-1)y\\
x^3 D^3 y= D_1 (D_1-1)(D_1-2)y\\
x^n D^n y= D_1 (D_1-1)(D_1-2)\cdots (D_1-n+1)y\\
\end{array}
$$

#### 3.وبالتعويض نحصل علي معادلة خطية في $t$ 
#### 4.نوجد الحل المكمل والخاص على صورة $y_c(t)$ و $y_p(t)$
#### 5.التعويض مجددا للحصول علي $y_c(x)$ و $y_p(x)$:

$$
e^t = x \quad,\qquad t = \ln x
$$

## طريقة فروبينيس
تكون لمعادلة من الرتبة الثانية على الشكل:

$$
\color{#a7c957}\large a_0(x)y'' +a_1(x)y' + a_2(x)y = 0
$$

ويعطى نقطة $x=x_0$ لإيجاد الحل بالقرب منها
### نوع النقطة
#### منتظمة
تحقق شرط أن:

$$
\large\lim_{x\rightarrow x_0} \dfrac{a_1(x)}{a_0(x)} \quad,\quad \lim_{x\rightarrow x_0} \dfrac{a_2(x)}{a_0(x)}
$$

 كميات محددة (لا تساوي $\pm\infty$)
#### شاذة منتظمة
تحقق

$$
\large\lim_{x\rightarrow x_0} (x - x_0) \dfrac{a_1(x)}{a_0(x)} \quad,\quad \lim_{x\rightarrow x_0} (x - x_0)^2 \dfrac{a_2(x)}{a_0(x)}
$$

 كميات محددة (لا تساوي $\pm\infty$)
#### شاذة غير منتظمة
لم تحقق ايا مما سبق

### خطوات الحل
تستخدم طريقة فروبينيس في حالة النقطة **منتظمة** أو **الشاذة منتظمة**

#### فرض الحل على صورة:

$$
\large y(x) = \sum_{n=0}^\infty c_n(x-x_0)^{r+n}
$$

#### ومنه نستنتج أن:

$$
\large y'(x) = \sum_{n=0}^\infty c_n (r+n)(x-x_0)^{r+n-1}
$$

$$
\large y''(x) = \sum_{n=0}^\infty c_n (r+n)(r+n-1)(x-x_0)^{r+n-2}
$$

#### التعويض في المعادلة الأصلية ثم تجميع الحدود المتشابهة و مقارنة المعاملات

$$
\large\begin{align}
 & a_0(x)\sum_{n=0}^\infty c_n (r+n)(r+n-1)(x-x_0)^{r+n-2}\\
+\,& a_1(x)\sum_{n=0}^\infty c_n (r+n)(x-x_0)^{r+n-1}\\
+\,& a_2(x)\sum_{n=0}^\infty c_n(x-x_0)^{r+n} = 0
\end{align}
$$

#### مساواة معامل اصغر قوى بصفر
اي عند n = 0 , تكون المعادلة على هذا الشكل:

$$
c_0\,\phi_1(r)\,\phi_2(r) = 0
$$

#### إيجاد قيم $r$:
بما أن $c_0 \ne 0$ فإنه ينتج حلين أو حل على الأكثر لـ $r$ .
#### مساواة معامل الحد العام $n$ بصفر:
فتتكون علاقة بين $c_{n+1}$ , $c_n$ 
#### التعويض بقيمة من $r$ وبقيم $c_1 , c_2 , c_3 , c_4$ 
ثم التعويض في المعادلة الأصلية $y(x)$ حتى تتكون معادلة في ثابت واحد $c_0$
# تحويل لابلاس "Laplace transform" :
تحويل لابلاس لدالة $F(t)$ ينتج عنه دالة أخرى $f(s)$ حيث:

$$
\color{#a7c957}\large L\{\,F(t)\,\} = \int_0^\infty e^{-st}F(t)dt = f(s)
$$

لا توجد طريقة لإيجاد معكوس لابلاس $L^{-1}$ لدالة, فيفضل حفظ تحويلات الدوال المشهورة:

$$
\large\begin{array}{l|l|l}
F(t) & f(s) = \mathcal{L}\{F(t)\} & \text{Condition} \\
\hline
1 & \dfrac{1}{s} & s > 0 \\
t^n & \dfrac{n!}{s^{n+1}} = \dfrac{\Gamma(n+1)}{s^{n+1}} \qquad & s > 0 \\
e^{at} & \dfrac{1}{s-a} & s > a \\
\sin bt & \dfrac{b}{s^2+b^2} & s > 0 \\
\cos bt & \dfrac{s}{s^2+b^2} & s > 0 \\
\sinh bt & \dfrac{b}{s^2-b^2} & s > |a| \\
\cosh bt & \dfrac{s}{s^2-b^2} & s > |a| \\
\end{array}
$$

## خواص هامة:

$$
\large1) \quad \begin{array}{l}
L\{F'(t)\} = sf(s) - F(0)\\
L\{F''(t)\} = s^2f(s) - sF(0) - F'(0)\\
L\{F^{(n)}(t)\} = s^nf(s) - s^{n-1}F(0)  - s^{n-2}F'(0) - \cdots - sF^{n-2}(0) - F^{n-1}(0)\\
\end{array}
$$

$$
\large2) \qquad L\{\,e^{at} F(t)\,\} = f(s-a)
$$

$$
\large3) \qquad L\{\,t^{n} F(t)\,\} = (-1)^n \dfrac{d^n}{ds^n}[\,f(s)\,]
$$

$$
\large\begin{array}{l|l l}
F(t) & f(s)\\
\hline
t^n e^{at} & \dfrac{n!}{(s-a)^{n+1}}\\
t\sin bt & \dfrac{2\,sb}{(s^2 + b^2)^2}\\
t\cos bt & \dfrac{s^2-b^2}{(s^2 + b^2)^2}\\
e^{at}\sin bt & \dfrac{b}{(s-a)^2 + b^2}\\
e^{at}\cos bt & \dfrac{s-a}{(s-a)^2 + b^2}\\
\end{array}
$$

# دالتا جاما وبيتا "Gamma & Beta functions" :
## دالة جاما:
لإجاد تكامل $\displaystyle\int_0^\infty x e ^{-x} dx$ نقوم بالتجزئة مرة واحدة.
<br>
ولإجاد تكامل $\displaystyle\int_0^\infty x^n e ^{-x} dx$ نقوم بالتجزئة $n$ مرة.
دالة جاما تقوم بحاسب التكامل على مرة واحدة لأي قيمة $n$ أكبر من 0 **حتى إذا كانت كسرا**
### التعريف
#### بالتكامل:

$$
\Gamma(x) = \int_o^\infty  u^{x-1} e^{-u}du
$$

#### بالنهايات:

$$
\Gamma(x) = \lim_{n\rightarrow \infty}{\dfrac{n!\,n^x}{x(x+1)(x+2)\cdots(x+n)}}
$$

### خواص مميزة للدالة

$$
\begin{array}{l}
\Gamma(1) = 1\\
\Gamma\left(\dfrac12\right) = \sqrt{\pi}\\
\Gamma(x+1) = x\,\Gamma(x)\\
\Gamma(x+1) = x!\\
\Gamma(2x) = \dfrac{2^{2x-1}}{\sqrt\pi}\,\Gamma(x)\,\Gamma\left(x+\dfrac12\right)\\
\Gamma(x)\Gamma(1-x) = \dfrac{\pi}{\sin \pi x} \quad\text{for: } 0<x<1\\
\end{array}
$$

## دالة بيتا:

$$
\large\begin{align}
\beta(m,n)&=\int_0^1 x^{m-1}(1-x)^{n-1}\,dx\\
&=\int_0^\infty  \dfrac{x^{m-1}}{(1+x)^{m+n}}dx \\
&=2\int_0^{\pi/2}(\cos\theta)^{2m-1} (\sin\theta)^{2n-1} d\theta\\\\
&\quad\text{for: } n,m>0
\end{align}
$$

### خواص مميزة للدالة

$$
\begin{array}{l}
\beta(m,n) = \beta(n,m)\\
\beta(m,n) = \dfrac{\Gamma(m) \Gamma(n)}{\Gamma(m+n)}\\
\beta(m,n) = \dfrac{(m-1)! (n-1)!}{(m+n-1)!}\\[5px]
\beta(1,1) = 1 \qquad \beta\left(\dfrac12,\dfrac12\right) = \pi
\end{array}
$$

# كثيرات حدود شيبيشيف
تذكر أن:

$$
e^{i\theta} = \cos\theta + i \sin\theta
$$

$$
\begin{align}
\sin^2\theta+ \cos^2\theta = 1 \quad &\Rightarrow \;\sin\theta = \pm\sqrt{1-\cos^2\theta}\\
&\Rightarrow\;\cos\theta = \pm\sqrt{1-\sin^2\theta}
\end{align}
$$

$$
\sin(a\pm b) = \sin a \cos b \pm \cos a \sin b \quad:\quad \sin2a = s\sin a \cos a
$$

$$
\cos(a\pm b)=\cos a \cos b \mp \sin a \sin b \;:\; \cos 2a = \cos^2 a  -\sin^2 a
$$

$$
\large\cos\theta = \dfrac{e^{i\theta}+e^{-i\theta}}{2} \qquad,\qquad \sin\theta = \dfrac{e^{i\theta}-e^{-i\theta}}{2i}
$$

## المعادلة

$$
\color{#a7c957}\large (1-x^2)y'' - xy' + n^2y = 0
$$

يوجد نوعان للحل (*حيث: $n\in Z^+$*)
### النوع الأول: $y = T_n(x)$ 

$$
T_n(x) = \cos(n\cos^{-1}x)
$$

#### الصورة المركبة

$$
T_n(x) = \dfrac12 \left( \left(x+i\sqrt{1-x^2}\right)^n - \left(x-i\sqrt{1-x^2}\right)^n \right)
$$

#### حالات خاصة:

$$
\begin{array}{l}
T_0(x) = 1\\
T_1(x) = x\\
T_2(x) = 2x^2-1\\
T_3(x) = 4x^3 - 3x\\
\end{array}
$$

### النوع الثاني: $y = U_n(x)$ 

$$
U_n(x) =\sin(n\cos^{-1}x)
$$

$$
U_n(x) = \dfrac{\sin\left((n+1) cos^{-1}x\right)}{\sqrt{1-x^2}}
$$

#### الصورة المركبة

$$
U_n(x) = \dfrac{-i}{2} \left( \left(x+i\sqrt{1-x^2}\right)^n - \left(x-i\sqrt{1-x^2}\right)^n \right)
$$

#### حالات خاصة:

$$
\begin{array}{l}
U_0(x) = 1\\
U_1(x) = \sqrt{1-x^2}\\
U_2(x) = \sqrt{1-x^2}\;\cdot2x\\
U_3(x) = \sqrt{1-x^2}\,(4x^2-1)\\
\end{array}
$$
