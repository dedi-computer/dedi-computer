<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Dedi Computer - Jasa Perbaikan Elektronik Profesional</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />
</head>
<body class="bg-gray-50 text-gray-800">
  <!-- Header -->
  <header class="bg-blue-600 text-white p-6 shadow-lg">
    <div class="container mx-auto flex justify-between items-center">
      <h1 class="text-2xl font-bold">Dedi Computer</h1>
      <nav class="space-x-6">
        <a href="#home" class="hover:underline">Beranda</a>
        <a href="#layanan" class="hover:underline">Layanan</a>
        <a href="#tentang" class="hover:underline">Tentang</a>
        <a href="#kontak" class="hover:underline">Kontak</a>
      </nav>
    </div>
  </header>

  <!-- Hero Section -->
  <section id="home" class="text-center py-20 bg-gradient-to-r from-blue-600 to-blue-400 text-white">
    <h2 class="text-4xl font-bold mb-4">Solusi Profesional untuk Segala Masalah Elektronik Anda</h2>
    <p class="text-lg mb-6">Kami siap memperbaiki laptop, TV, kulkas, HP, dan perangkat elektronik lainnya dengan cepat dan bergaransi.</p>
    <a href="#kontak" class="bg-white text-blue-600 font-semibold py-3 px-6 rounded-full shadow hover:bg-gray-100 transition">Hubungi Kami</a>
  </section>

  <!-- Layanan -->
  <section id="layanan" class="py-16 container mx-auto text-center">
    <h3 class="text-3xl font-bold mb-10">Layanan Kami</h3>
    <div class="grid md:grid-cols-3 gap-8">
      <div class="bg-white p-6 rounded-2xl shadow hover:shadow-lg transition">
        <i class="fas fa-laptop text-blue-600 text-4xl mb-4"></i>
        <h4 class="text-xl font-semibold mb-2">Perbaikan Laptop & Komputer</h4>
        <p>Instal ulang, ganti sparepart, dan perbaikan sistem cepat dan bergaransi.</p>
      </div>
      <div class="bg-white p-6 rounded-2xl shadow hover:shadow-lg transition">
        <i class="fas fa-tv text-blue-600 text-4xl mb-4"></i>
        <h4 class="text-xl font-semibold mb-2">Servis TV & Audio</h4>
        <p>Perbaikan layar, suara, dan sistem TV LED/LCD berbagai merk.</p>
      </div>
      <div class="bg-white p-6 rounded-2xl shadow hover:shadow-lg transition">
        <i class="fas fa-blender text-blue-600 text-4xl mb-4"></i>
        <h4 class="text-xl font-semibold mb-2">Perbaikan Alat Rumah Tangga</h4>
        <p>Kulkas, mesin cuci, kipas, dispenser, dan peralatan elektronik lainnya.</p>
      </div>
    </div>
  </section>

  <!-- Tentang -->
  <section id="tentang" class="bg-gray-100 py-16">
    <div class="container mx-auto text-center">
      <h3 class="text-3xl font-bold mb-6">Tentang Kami</h3>
      <p class="max-w-2xl mx-auto">Dedi Computer berlokasi di Alam Barajo, Jambi. Kami berpengalaman dalam perbaikan berbagai perangkat elektronik dengan teknisi profesional dan layanan bergaransi. Kepuasan pelanggan adalah prioritas utama kami.</p>
    </div>
  </section>

  <!-- Kontak -->
  <section id="kontak" class="py-16 container mx-auto">
    <h3 class="text-3xl font-bold text-center mb-8">Hubungi Kami</h3>
    <div class="max-w-xl mx-auto bg-white p-8 rounded-2xl shadow">
      <form id="serviceForm" class="space-y-4">
        <div>
          <label class="block font-semibold mb-1">Nama</label>
          <input type="text" id="nama" class="w-full border rounded-lg p-2" placeholder="Nama Anda" required>
        </div>
        <div>
          <label class="block font-semibold mb-1">Nomor Telepon</label>
          <input type="text" id="telepon" class="w-full border rounded-lg p-2" placeholder="08xxxxxxxxxx" required>
        </div>
        <div>
          <label class="block font-semibold mb-1">Jenis Barang</label>
          <input type="text" id="barang" class="w-full border rounded-lg p-2" placeholder="Contoh: Laptop Asus" required>
        </div>
        <div>
          <label class="block font-semibold mb-1">Deskripsi Kerusakan</label>
          <textarea id="deskripsi" class="w-full border rounded-lg p-2" rows="3" placeholder="Jelaskan kerusakan perangkat Anda" required></textarea>
        </div>
        <div class="flex justify-center space-x-4 pt-4">
          <!-- Tombol WhatsApp -->
          <button type="button" onclick="kirimWhatsApp()" class="flex items-center space-x-2 bg-green-500 hover:bg-green-600 text-white font-semibold py-2 px-4 rounded-full transition">
            <i class="fab fa-whatsapp"></i>
            <span>Kirim via WhatsApp</span>
          </button>
          <!-- Tombol Email -->
          <button type="submit" class="flex items-center space-x-2 bg-blue-500 hover:bg-blue-600 text-white font-semibold py-2 px-4 rounded-full transition">
            <i class="fas fa-envelope"></i>
            <span>Kirim via Email</span>
          </button>
        </div>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-blue-600 text-white text-center py-4 mt-16">
    <p>© 2025 Dedi Computer | Jasa Servis Elektronik Jambi | Telp: 082371731189</p>
  </footer>

  <script>
    function kirimWhatsApp() {
      const nama = document.getElementById('nama').value;
      const telepon = document.getElementById('telepon').value;
      const barang = document.getElementById('barang').value;
      const deskripsi = document.getElementById('deskripsi').value;
      const pesan = `Halo Dedi Computer, saya *${nama}* (${telepon}).%0ASaya ingin servis *${barang}* dengan masalah: %0A${deskripsi}`;
      window.open(`https://wa.me/6282371731189?text=${pesan}`, '_blank');
    }

    document.getElementById('serviceForm').addEventListener('submit', function(e) {
      e.preventDefault();
      const data = {
        nama: document.getElementById('nama').value,
        telepon: document.getElementById('telepon').value,
        barang: document.getElementById('barang').value,
        deskripsi: document.getElementById('deskripsi').value
      };

      fetch('https://formspree.io/f/mzzbqpzl', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(data)
      }).then(response => {
        alert('Pesan berhasil dikirim ke email Dedi Computer!');
        document.getElementById('serviceForm').reset();
      }).catch(error => {
        alert('Terjadi kesalahan, silakan coba lagi.');
      });
    });
  </script>
</body>
</html>
