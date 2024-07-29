#dev@mukhamedzhan_dyr


from .. import loader, utils
import asyncio


class IrisfarmMod(loader.Module):
    """Автоматизирует работу с айзен соло (автоматическая ферма)"""

    strings = {"name": "FARMcard"}

    async def farmcmd(self, message):
        """Начинает автоматический фарм. """
        self.set("farm", True)
        while self.get("карта"):
            await message.reply("/twist")
            await asyncio.sleep(14700)

    async def unfarmcmd(self, message):
        """Выключает автоферму."""
        self.set("farm", False)
        await utils.answer(
            message,
            "❗️ <b>Автоферма выключена.</b>",
        )
