# Calorie-Counter
This application is programmed with Visual Basic and built in Visual Studios. This application calculates how many calories someone has burnt during certain exercises. 

Public Class Form1

    Private Sub Button1_Click(sender As System.Object, e As System.EventArgs) Handles Button1.Click
        Dim scycling As String
        Dim srunning As String
        Dim sswim As String
        Dim cycling As Double
        Dim running As Double
        Dim swim As Double
        Dim weightloss As Double
        scycling = txtcycle.Text
        srunning = txtrun.Text
        sswim = txtswim.Text
        cycling = Double.Parse(scycling)
        running = Double.Parse(srunning)
        swim = Double.Parse(sswim)
        weightloss = ((cycling * 200) + (running * 475) + (swim * 275)) / 3500
        txtloss.Text = weightloss & " pounds were lost"
    End Sub
End Class
