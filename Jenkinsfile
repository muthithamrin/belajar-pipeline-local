pipeline {
    agent any
    
    environment {
        // Tentukan path lokal tempat Anda ingin melakukan clone repository
        LOCAL_CLONE_PATH = "/Users/muthithamrin/documents"
    }
    
    stages {
        stage('Clone Repository') {
            steps {
                // Menghapus folder repository jika sudah ada sebelumnya
                deleteDir()
                
                // Membuat folder untuk clone repository
                dir(Jenkins-pipeline-coba-clone-by-jenkins) {
                    // Melakukan clone dari repository GitHub
                    git branch: 'main', url: 'https://github.com/muthithamrin/belajar-pipeline-local.git'
                }
            }
        }
        // Tambahkan tahapan-tahapan lain sesuai kebutuhan Anda
    }

    // Tambahkan post-build actions jika diperlukan
    post {
        always {
            // Tambahkan langkah-langkah yang perlu dijalankan setelah pipeline selesai
        }
    }
}
