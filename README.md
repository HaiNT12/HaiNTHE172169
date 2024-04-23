This is Project from SWP391.

I. Code Rules

Model is package just inlcude object from Table (same attributes) e.g model/User.java

Change MSSQL name and Database name in DAO/DBContext.java

You can read description below to understand DAO file or read file DAO/DAOUser.java

DAO file includes functions get data from database

In every file DAO, must "extends DBContext", and copy code: PreparedStatement pstm; Connection cnn; ResultSet rs;

public DAOUser() { connect(); }

public void connect() { cnn = super.connection; }

in try/catch must inlcude 2 catching: catch (SQLException e) { System.out.println("SQL <name_function>: " + e.getMessage()); return //your_failure_value; } catch (Exception e) { System.out.println("<name_function>: " + e.getMessage()); return //your_failure_value; }

Trong css, đặt tên class, id phải rõ ràng, ghi rõ chức năng của nó, tránh nhầm lẫn với ae khác, ko đc đặt tên chung như title, container,... phải ghi cụ thể nó có chức vụ gì
