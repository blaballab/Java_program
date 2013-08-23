package me.luka.hello;

import java.util.logging.Logger;
import org.bukkit.ChatColor;
import org.bukkit.GameMode;
import org.bukkit.command.Command;
import org.bukkit.command.CommandSender;
import org.bukkit.entity.Player;
import org.bukkit.plugin.java.JavaPlugin;

public class Main extends JavaPlugin { 
	public final Logger logger = Logger.getLogger("Minecraft");

	public void onEnable() {
		logger.info(" ");
		logger.info("Luka plugin has been enabled");
		logger.info(" ");
		getServer().getWorld("World").setSpawnLocation(331, 4, -390);
		this.saveDefaultConfig();
		
	}
	public void onDisable() {
		logger.info("Luka plugin has been disabled");
	}
