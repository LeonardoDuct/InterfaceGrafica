# InterfaceGrafica
Projeto da materia de POO II
package view;

import java.awt.BorderLayout;
import java.awt.EventQueue;

import javax.swing.JFrame;
import javax.swing.JPanel;
import javax.swing.border.EmptyBorder;
import javax.swing.JButton;
import java.awt.event.ActionListener;
import java.awt.event.ActionEvent;
import javax.swing.JTextField;
import javax.swing.JLabel;
import javax.swing.JOptionPane;
import javax.swing.JComboBox;
import javax.swing.DefaultComboBoxModel;

public class ViewDesafio extends JFrame {

	protected static final String DadosSalvos = null;
	private JPanel contentPane;
	private JTextField textField;
	private JTextField textField_1;
	private JTextField textField_3;
	private JTextField textField_5;
	private JTextField textField_2;

	/**
	 * Launch the application.
	 */
	public static void main(String[] args) {
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					ViewDesafio frame = new ViewDesafio();
					frame.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	/**
	 * Create the frame.
	 */
	public ViewDesafio() {
		setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		setBounds(100, 100, 495, 533);
		contentPane = new JPanel();
		contentPane.setBorder(new EmptyBorder(5, 5, 5, 5));
		setContentPane(contentPane);
		contentPane.setLayout(null);
		
		JButton btnNewButton = new JButton("Inserir");
		btnNewButton.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				
				String txtNome = DadosSalvos;
				JOptionPane.showMessageDialog(null, "DadosSalvos: "+txtNome);
			}
		});
		btnNewButton.setBounds(123, 389, 101, 35);
		contentPane.add(btnNewButton);
		
		JButton btnNewButton_1 = new JButton("Cancelar");
		btnNewButton_1.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
			}
		});
		btnNewButton_1.setBounds(233, 389, 101, 35);
		contentPane.add(btnNewButton_1);
		
		textField = new JTextField();
		textField.setBounds(71, 73, 206, 20);
		contentPane.add(textField);
		textField.setColumns(10);
		
		textField_1 = new JTextField();
		textField_1.setToolTipText("");
		textField_1.setBounds(71, 187, 86, 20);
		contentPane.add(textField_1);
		textField_1.setColumns(10);
		
		JLabel txtNome = new JLabel("Nome e Sobrenome");
		txtNome.setBounds(73, 48, 112, 14);
		contentPane.add(txtNome);
		
		textField_3 = new JTextField();
		textField_3.setBounds(365, 73, 86, 20);
		contentPane.add(textField_3);
		textField_3.setColumns(10);
		
		JComboBox comboBox = new JComboBox();
		comboBox.setModel(new DefaultComboBoxModel(new String[] {"<Fator RH>]", "Positivo", "Negativo"}));
		comboBox.setBounds(310, 248, 101, 22);
		contentPane.add(comboBox);
		
		JLabel lbltipoS = new JLabel("Tipo Sangu\u00EDneo");
		lbltipoS.setBounds(71, 252, 73, 14);
		contentPane.add(lbltipoS);
		
		textField_5 = new JTextField();
		textField_5.setBounds(71, 308, 86, 20);
		contentPane.add(textField_5);
		textField_5.setColumns(10);
		
		JLabel lblNewLabel_3 = new JLabel("Curso Atual");
		lblNewLabel_3.setBounds(71, 283, 86, 14);
		contentPane.add(lblNewLabel_3);
		
		JComboBox comboBox_1 = new JComboBox();
		comboBox_1.setModel(new DefaultComboBoxModel(new String[] {"< Selecione uma das Op\u00E7\u00F5es >", "Tipo A", "Tipo B", "Tipo AB", "Tipo O"}));
		comboBox_1.setBounds(204, 248, 96, 22);
		contentPane.add(comboBox_1);
		
		JLabel lblNewLabel_5 = new JLabel("Endere\u00E7o");
		lblNewLabel_5.setBounds(68, 160, 133, 14);
		contentPane.add(lblNewLabel_5);
		
		JComboBox comboBox_2 = new JComboBox();
		comboBox_2.setModel(new DefaultComboBoxModel(new String[] {"<DD>", "11", "46", "33", "41", "96", "98"}));
		comboBox_2.setBounds(288, 72, 67, 22);
		contentPane.add(comboBox_2);
		
		textField_2 = new JTextField();
		textField_2.setBounds(71, 131, 86, 20);
		contentPane.add(textField_2);
		textField_2.setColumns(10);
		
		JLabel lblNewLabel_1 = new JLabel("CEP");
		lblNewLabel_1.setBounds(71, 116, 46, 14);
		contentPane.add(lblNewLabel_1);
		
		JLabel lblNewLabel_2 = new JLabel("Contato");
		lblNewLabel_2.setBounds(288, 48, 46, 14);
		contentPane.add(lblNewLabel_2);
		
		JComboBox comboBox_3 = new JComboBox();
		comboBox_3.setModel(new DefaultComboBoxModel(new String[] {"< SEMESTRE >", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10"}));
		comboBox_3.setBounds(176, 307, 101, 22);
		contentPane.add(comboBox_3);
	}
}
