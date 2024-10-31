public class Mahasiswa {
    int nim;
    String nama;
    char kelas;
    String prodi;
    String alamat;

    // Konstruktor
    public Mahasiswa(int nim, String nama, char kelas, String prodi, String alamat) {
        this.nim = nim;
        this.nama = nama;
        this.kelas = kelas;
        this.prodi = prodi;
        this.alamat = alamat;
    }

    // void
    public void tampilkanData() {
        System.out.println("NIM: " + nim);
        System.out.println("Nama: " + nama);
        System.out.println("Kelas: " + kelas);
        System.out.println("Program Studi: " + prodi);
        System.out.println("Alamat: " + alamat);
    }

    // return
    public String ambilNama() {
        return this.nama;
    }

    // parameter
    public void ubahAlamat(String alamatBaru) {
        this.alamat = alamatBaru;
    }

    // parameter
    public void ubahProdi(String prodiBaru) {
        this.prodi = prodiBaru;
    }

    // parameter
    public void ubahNim(int nimBaru) {
        this.nim = nimBaru;
    }

    // parameter
    public void ubahKelas(char kelasBaru) {
        this.kelas = kelasBaru;
    }

    public static void main(String[] args) {
       
        Mahasiswa mhs = new Mahasiswa(23533821, "Ayuu", 'C', "Teknik Informatika", "Magetan");
        
        // Menampilkan data awal mahasiswa
        System.out.println("Data Mahasiswa Sebelum Perubahan:");
        mhs.tampilkanData();
        
        // Mengubah beberapa data mahasiswa
        mhs.ubahAlamat("Siman");
        mhs.ubahProdi("Keperawatan");
        mhs.ubahNim(23533901);
        mhs.ubahKelas('D');

        // Menampilkan data setelah perubahan
        System.out.println("\nData Mahasiswa Setelah Perubahan:");
        mhs.tampilkanData();
    }
}
