# inventaris
1.**jmenu
 String username = txtUsername.getText();
        String password = String.valueOf(txtPassword.getPassword());
        
        // Data Login admin
        String validUsernameadmin = "admin";
        String validPasswordadmin = "1234";
        
        // Data Login staf
        String validUsernameStaf = "staf";
        String validPasswordStaf = "5678";
        
        
        if (username.equals(validUsernameadmin)  && password.equals(validPasswordadmin)) {
           //Login admin berhasil
           JOptionPane.showMessageDialog(this,"Login Berhasil!", "Sukses", JOptionPane.INFORMATION_MESSAGE);
           Dassboard newWin = new Dassboard();
           newWin.setVisible(true);
           this.dispose();
        } else if (username.equals(validUsernameStaf) && password.equals(validPasswordStaf)) {
            //Login staf berhasil
            JOptionPane.showMessageDialog(this, "Login Staf Berhasil!", "Sukses", JOptionPane.INFORMATION_MESSAGE);
            Dassboard newWin = new Dassboard();
            newWin.setVisible(true);
            this.dispose();
        } else {
            JOptionPane.showMessageDialog(this, "Username atau password salah!", "Gagal", JOptionPane.ERROR_MESSAGE);
            txtUsername.setText("");
            txtPassword.setText("");
        }                    
    }                                         
