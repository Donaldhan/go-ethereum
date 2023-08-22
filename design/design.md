geth main.go


ethclient.go

eth_getLogs：FilterLogs


# rpc server api

api.go:getLogs


 (f *Filter) Logs(ctx context.Context) ([]*types.Log, error) 

 func (api *FilterAPI) GetLogs(ctx context.Context, crit FilterCriteria) ([]*types.Log, error)


# 以太坊节点
backend.go

1. 创建以太坊节点
func New(stack *node.Node, config *ethconfig.Config) (*Ethereum, error)

2. 开始挖矿
func (s *Ethereum) StartMining() error

> 节点服务
node.go
func New(conf *Config) (*Node, error) 



> 区块同步
sync.go
 func (h *handler) doSync(op *chainSyncOp) 

