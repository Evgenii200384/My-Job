from raffaelo.contracts.erc20.contract import ERC20TokenContract
from raffaelo.providers.http.provider import HTTPProvider


address = '0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48'
provider = HTTPProvider(uri='https://rpc.ankr.com/eth')

usdc = ERC20TokenContract(address=address)
