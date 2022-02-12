# 386.-FXML-Config-387.-Adicionar-Controles
Tela de login parte 1
ARQUIVO FXML
__________________________________________
<?xml version="1.0" encoding="UTF-8"?>

<?import javafx.scene.layout.*?>
<?import javafx.scene.control.*?>

<GridPane xmlns:fx="http://javafx.com/fxml/1">
	
	<Label text="Seja Bem Vindo"
		GridPane.columnIndex="0" GridPane.rowIndex="0"></Label>
		
	<Label text="E-mail: "
	    GridPane.columnIndex="0" GridPane.rowIndex="1"></Label>
	
	<TextField
		GridPane.columnIndex="1" GridPane.rowIndex="1">
	</TextField>
	
	<Label text="Senha: "
		GridPane.columnIndex="0" GridPane.rowIndex="2"></Label>
	<PasswordField
		GridPane.columnIndex="1" GridPane.rowIndex="2">
	</PasswordField>
	<Button text = "Entrar"
		GridPane.columnIndex="0" GridPane.rowIndex="3">
	
	</Button>
</GridPane>
__________________________________________
O APP
__________________________________________
public class AppFXML extends Application {
	
	@Override
	public void start(Stage primaryStage) throws Exception {
		URL arquivoFXML = getClass().getResource("/fxml/Login.fxml");
		GridPane raiz = FXMLLoader.load(arquivoFXML);
		
		Scene cena = new Scene(raiz, 350, 400);
		
		primaryStage.setResizable(false);
		primaryStage.setTitle("Tela de Loguin");
		primaryStage.setScene(cena);
		primaryStage.show();
	}
	public static void main(String [] args) {
		launch(args);
	}
}
![image](https://user-images.githubusercontent.com/95525963/153729850-5958bffb-bf50-404d-9fb5-ec6b390c1e62.png)
