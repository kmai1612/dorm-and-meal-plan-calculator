Public Class frmMain
    Private Sub frmMain_Load(sender As Object, e As EventArgs) Handles MyBase.Load

        'Display the Dormitory price in the list box
        lstDormitories.Items.Add("Allen Hall - 2,500.00 ")
        lstDormitories.Items.Add("Pike Hall - 2,200.00")
        lstDormitories.Items.Add("Farthing Hall - 2,100.00")
        lstDormitories.Items.Add("UniversitySuites - 2,800.00")

    End Sub

    Private Sub btnAddDormitory_Click(sender As Object, e As EventArgs) Handles btnAddDormitory.Click

        ' if user don't choose any price in list box 
        Select Case lstDormitories.SelectedIndex
            Case -1
                MessageBox.Show("Select A Dormitory Please!")
        End Select

        'Determine the value in Module and display the value of price to lblDormitory 
        Select Case lstDormitories.SelectedIndex
            Case 0
                lblDormitory.Text = mdlSample.Allen_Hall.ToString("c2")
            Case 1
                lblDormitory.Text = mdlSample.Pike_Hall.ToString("c2")
            Case 2
                lblDormitory.Text = mdlSample.Farthing_Hall.ToString("c2")
            Case 3
                lblDormitory.Text = mdlSample.UniversitySuites.ToString("c2")
        End Select

    End Sub

    Private Sub btnViewMP_Click(sender As Object, e As EventArgs) Handles btnViewMP.Click
        'Display the second form (Meal Plan)
        Me.Hide()
        frmMealPlans.Show()

    End Sub

    Private Sub btnClear_Click(sender As Object, e As EventArgs) Handles btnClear.Click

        'Clear all the label except the list box
        lblDormitory.Text = String.Empty
        lblMeal_Plan.Text = String.Empty
        lblTotal.Text = String.Empty

    End Sub

    Private Sub btnExit_Click(sender As Object, e As EventArgs) Handles btnExit.Click

        ' Exit Program 
        Application.Exit()

    End Sub
End Class
