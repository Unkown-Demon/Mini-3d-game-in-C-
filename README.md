# 🎮 Mini 3D Game in C++

Ushbu loyiha C++ va OpenGL yordamida yaratilgan oddiy 3D o'yincha (mini-o'yin) bo'lib, 3D grafikani renderlashning asosiy tamoyillarini namoyish etadi. Loyiha aylanuvchi rangli kubni ko'rsatadi va foydalanuvchiga kamera orqali sahnada harakatlanish imkonini beradi.

## 🌟 Asosiy Xususiyatlar

*   **Platforma:** C++ (C++17 standarti)
*   **Grafika API:** OpenGL 3.3 Core Profile
*   **Kutubxonalar:**
    *   **GLFW:** Oyna yaratish va kirish (klaviatura) boshqaruvi uchun.
    *   **GLEW:** OpenGL funksiyalarini yuklash uchun.
    *   **GLM:** OpenGL uchun matematik operatsiyalar (matritsalar, vektorlar) uchun.
*   **Build Tizimi:** CMake
*   **O'yin Elementi:** WASD tugmalari yordamida boshqariladigan erkin kamera harakati.

## 🛠️ Loyihani Qurish

Loyihani qurish va ishga tushirish uchun sizga C++ kompilyatori (masalan, GCC/G++), CMake va yuqorida sanab o'tilgan OpenGL kutubxonalari kerak bo'ladi.

### 1. Talablarni O'rnatish

Debian/Ubuntu tizimlari uchun kerakli kutubxonalarni o'rnatish:

```bash
sudo apt update
sudo apt install build-essential cmake libglfw3-dev libglew-dev libglm-dev
```

### 2. Loyihani Klonlash

Loyihani mahalliy kompyuteringizga klonlang:

```bash
git clone https://github.com/Unkown-Demon/Mini-3d-game-in-C-.git
cd Mini-3d-game-in-C-
```

### 3. Qurish (Build)

Loyihani CMake yordamida qurish:

```bash
# Build katalogini yaratish
mkdir build
cd build

# CMake yordamida loyihani sozlash
cmake ..

# Loyihani qurish
make
```

### 4. Ishga Tushirish

Qurilgan dastur `build/bin/` katalogida joylashgan bo'ladi.

```bash
# Dasturni ishga tushirish
./bin/Simple3DGame
```

## 🕹️ Boshqaruv

| Tugma | Harakat |
| :---: | :---: |
| **W** | Oldinga harakatlanish |
| **S** | Orqaga harakatlanish |
| **A** | Chapga harakatlanish |
| **D** | O'ngga harakatlanish |
| **ESC** | Dasturni yopish |

## 📂 Loyiha Tuzilmasi

```
Mini-3d-game-in-C-/
├── CMakeLists.txt      # CMake konfiguratsiya fayli
├── README.md           # Ushbu fayl
├── shaders/
│   ├── fragment.glsl   # Fragment Shader kodi
│   └── vertex.glsl     # Vertex Shader kodi
└── src/
    └── main.cpp        # Asosiy C++ kodi (Oyna, Kub, Kamera mantiqi)
```

---
**Muallif:** Manus AI
**Litsenziya:** MIT (yoki mos keladigan litsenziya)
