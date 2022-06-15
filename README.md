# Web responsive
Tugas m3 dan m4

# Informasi Mahasiswa
Nama  : Akbar Zulfikar R
Nim   : 5190411163
Kelas : D

# Implementasi

# Route
Route::middleware('guest')->group(function (){
    Route::get('/login', [\App\Http\Controllers\AuthController::class, 'login'])->name('login');

    Route::post('/login', [\App\Http\Controllers\AuthController::class, 'authenticate']);
});

Route::middleware('auth')->group( function (){
    Route::get('/home', function () {
        return view('home');
    })->name('home');

    Route::get('/dosen', [\App\Http\Controllers\DosenController::class, 'index'])->name('dosen');

    Route::get('/mahasiswa', function () {
        return view('mahasiswa');
    })->name('mahasiswa');

    Route::get('/skripsi', function () {
        return view('skripsi');
    })->name('skripsi');

    Route::post('/logout', [\App\Http\Controllers\AuthController::class, 'logout'])->name('logout');
});

# Authetication 
Login, verification, dan logout diatur oleh controller 






