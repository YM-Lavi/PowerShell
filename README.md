# PowerShell
להשארת מסך דולק
while ($true) {
    Start-Process -FilePath "cmd.exe" -WindowStyle Minimized
    Start-Sleep -Seconds 1
    Get-Process cmd | Stop-Process -Force -ErrorAction SilentlyContinue
    Start-Sleep -Seconds 120
}
