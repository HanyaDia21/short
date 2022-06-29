# short
id = 5667  function punch(xx, yy)  pkt = {}  pkt.px = xx  pkt.py = yy  pkt.type = 3  pkt.value = 18  pkt.posX = GetLocal().posX pkt.posY = GetLocal().posY SendPacketRaw(1, pkt)  end  for _, obj in pairs(GetTile()) do if obj.fg == 5667 then pathfind(obj.x,obj.y) punch((GetLocal().posX / 32), (GetLocal().posY // 32)) end end
