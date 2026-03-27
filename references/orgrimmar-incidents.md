# Incident Response Reference

## Common Issues

### Agent Gateway Won't Start
- Check port conflicts: `lsof -i :PORT`
- Check logs: `journalctl -u openclaw-gateway -f`
- Restart: `openclaw gateway restart`

### Firebase Connection Issues
- Verify credentials: check SA key exists
- Test connectivity: `orgbus get agents`
- Check firewall rules

### Background Process Died
- Check if running: `pgrep -f PROCESS_NAME`
- Check logs for errors
- Restart the process
